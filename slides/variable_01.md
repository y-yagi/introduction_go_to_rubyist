
## 変数

* `var宣言`で変数を作成する

```
var name type = expression
```

```go
var s string
var i int
var s string = "string"
```
* 宣言時に値を指定しない場合、明示的にゼロ値で初期化される
  * 数値は0、ブーリアンはfalse, 文字列は"", 参照型はnil
  * 未初期化の変数というのは存在しない
