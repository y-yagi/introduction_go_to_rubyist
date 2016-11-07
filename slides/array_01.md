
## 配列

* 特定の型の0個以上の固定長列

```go
var a [3]int = [3]int{1, 2, 3}

fmt.Println(a[0]) // 1

for i, v := range a {
	fmt.Printf("%d: %d\n", i, v) // 0: 1, 1: 2, 2: 3
}
```
