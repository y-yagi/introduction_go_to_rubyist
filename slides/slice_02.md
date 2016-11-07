
## スライス

* 長さ: 配列の要素数
* 容量: 配列に最大追加出来る要素の数

```go
a := []int{0, 1, 2, 3, 4}
fmt.Println(len(a)) // 5
fmt.Println(cap(a)) // 5

a = append(a, 5)
fmt.Println(len(a)) // 6
fmt.Println(cap(a)) // 10
```
