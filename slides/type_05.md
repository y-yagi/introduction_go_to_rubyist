
## 型(文字列)

* 文字列中で式展開は出来ない
* 連結したい場合は`+`を使う、formatを使用して出力する、等を行う必要がある

```go
command := "hello"
const Usage = `This is usage message
Usage:
	%s yyy
`
fmt.Printf(Usage+"\n", command)
```
