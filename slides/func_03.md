
## 関数

* 先頭が大文字で始まる場合他のパッケージからアクセス可能
  * publicになる
  * これは関数以外に、型名、フィールド名等も同様

```go
package calc

func Sum(x, y int) int {
	return x + y
}

func subtraction(x, y int) int {
	return x - y
}
```

```go
fmt.Println(calc.Sum(1, 2))
fmt.Println(calc.subtraction(1, 2)) // "cannot refer to unexported name calc.subtractio"(コンパイル時にエラー)
```
