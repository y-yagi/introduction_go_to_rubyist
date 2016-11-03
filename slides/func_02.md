
## 関数

* Goでは関数はファーストクラス値
* 変数に代入したり、関数へ渡したり、関数から返したり出来る

```
func negative(x int) int { return -x }
func add1(r rune) rune   { return r + 1 }

func main() {
	n := negative
	fmt.Println(n(3))                          // -3
	fmt.Println(strings.Map(add1, "HAL-9000")) // IMB.:111
	fmt.Println(strings.Map(func(r rune) rune { return r + 1 }, "HAL-9000")) // 無名関数も使える
}
```
