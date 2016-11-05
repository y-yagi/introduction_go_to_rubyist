
## Web API

* http処理用のライブラリが標準に含まれているので、簡単にHTTPサーバを作る事が出来る

```go
package main

import (
	"fmt"
	"log"
	"net/http"
)

func handler(w http.ResponseWriter, r *http.Request) {
	fmt.Fprintf(w, "%v", r.URL.Path)
}

func main() {
	http.HandleFunc("/", handler)
	log.Fatal(http.ListenAndServe("localhost:3000", nil))
}
```
