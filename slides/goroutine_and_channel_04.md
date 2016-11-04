
## goroutine / channel

```go
package main

import (
	"fmt"
	"io"
	"io/ioutil"
	"net/http"
	"os"
	"time"
)

func fetch(url string, ch chan<- string) {
	start := time.Now()
	resp, err := http.Get(url)
	if err != nil {
		ch <- fmt.Sprint(err)
		return
	}
	defer resp.Body.Close()    // 後処理(ensureのようなイメージ)

	nbytes, err := io.Copy(ioutil.Discard, resp.Body)
	if err != nil {
		ch <- fmt.Sprintf("while reading %s: %v", url, err)
		return
	}
	secs := time.Since(start).Seconds()
	ch <- fmt.Sprintf("%.2fs %7d %s", secs, nbytes, url)   // 結果をchannelから送信
}

func main() {
	if len(os.Args) == 1 {
		fmt.Fprintln(os.Stderr, "Please specify url")
		os.Exit(1)
	}

	ch := make(chan string) // channelを作成(バッファ無し)
	for _, url := range os.Args[1:] {
		go fetch(url, ch)     // goroutineで動かす関数にchannelを渡す
	}

	for range os.Args[1:] {
		fmt.Println(<-ch)    // channelからのデータ受信を待つ
	}
}
```
