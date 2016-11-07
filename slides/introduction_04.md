
## Hello world

```go
package main    // コードが所属するパッケージ名の指定。必須。
                // なお、"main"パッケージは特別な意味があり、ライブラリではなく単独で動作する実行可能なプログラムを定義するために使用される

import "fmt"    // "fmt"パッケージの取り込み。"fmt"パッケージには入出力処理用の関数が定義されている。

func main() {   // "main"関数がエントリーポイント(最初に実行される)
	fmt.Println("Hello, world")  // "fmt"パッケージの"Println"関数の呼び出し
}
```
