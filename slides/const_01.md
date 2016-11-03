
## 定数

* 実行時ではなくコンパイル時に評価が行われることが保証されている式
* 定義した後に値を書き換える事は出来ない

```go
const pi = 3.14

const (
  e = 2.718
  pi = 3.14
)
```