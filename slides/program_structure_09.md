
## 定数

* 定数生成器(itoa)
* 関連した値の列を生成するのに使える
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
