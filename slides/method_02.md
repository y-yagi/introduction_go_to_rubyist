
## 構造体埋め込み

* 構造体に構造体を埋め込む事が出来る
  * "継承"っぽい事も出来なくも無い

```go
type Car struct {
	name string
}

func (c *Car) Run() string {
	return "run"
}

type Truck struct {
	Car             // "Car"に定義されているフィールド、メソッドがそのまま使える
	baggage string
}
```

```go
var truck Truck
truck.name = "alto"
truck.name // "alto"
```
