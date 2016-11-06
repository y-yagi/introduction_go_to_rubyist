
## メソッド

* Goでは型に対してメソッドを追加する事が出来る

```go
type User struct {
	firstName string
	lastName  string
}

func (u *User) FullName() string {
	return u.firstName + u.lastName
}
```

```go
taro := User{"Taro", "Ginza"}
fmt.Println(taro.FullName) // "TaroGinza"
```
* 構造体に対してメソッドを追加していくことでオブジェクト志向っぽいことも出来る
