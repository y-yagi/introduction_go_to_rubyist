
## 構造体

* 構造体のメンバーとして構造体を使用する事も可能

```go
type Address struct {
	zipCode    string
	prefecture string
}

type User struct {
	firstName string
	lastName  string
	email     string
	age       int
	address   Address
}

```

```go
taro := User{"Taro", "Ginza", "taro@example.com", 4, Address{"104-0061", "東京都"}}
fmt.Println(taro.firstName)
fmt.Println(taro.address.zipCode)
```
