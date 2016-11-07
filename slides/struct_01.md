
## 構造体

* 0個以上の任意の型の名前付き値を単一エンティティにまとめたもの

```go
type User struct {
	firstName string
	lastName  string
	email     string
	age       int
}
```

```go
taro := User{"Taro", "Ginza", "taro@example.com", 4}
fmt.Println(taro.firstName) // "Taro"
```
