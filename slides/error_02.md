
## エラー処理

* GoランタイムにError型というinterfaceが定義されており、それを使う

```go
type error interface {
    Error() string
}
```

* エラーが起きる可能性のある関数を定義する際は、必ず戻り値に`error`を含むようにする

```go
// os.Openメソッド
func Open(name string) (file *File, err error)
```

```go
f, err := os.Open("filename.ext")
if err != nil {
    log.Fatal(err)
}
```

