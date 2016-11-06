
## 定数

* 関連した値の列を生成するのに使える定数生成器(iota)という機能がある
  * ようはenum

```Go
type Weekday int

const (
  Sunday Weekday = iota
  Monday
  Tuesday
  Wednesday
  Thursday
  Friday
  Saturday
)
```
* `Sunday`は0、`Monday`は1、というように0始まりで設定される
