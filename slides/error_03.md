
## エラー処理

* 例外機構と設計の仕方を変える必要がある
* `error` interfaceは大分薄いinterfaceなので、そのまま使うのではなく、[pkgn/errors](https://godoc.org/github.com/pkg/errors)や独自の`error` typeを定義して、それを使う等の工夫があると良い
* 詳細は[Golangのエラー処理とpkg/errors](http://deeeet.com/writing/2016/04/25/go-pkg-errors/) や [Golang Error Handling lesson by Rob Pike](http://jxck.hatenablog.com/entry/golang-error-handling-lesson-by-rob-pike)を参照
