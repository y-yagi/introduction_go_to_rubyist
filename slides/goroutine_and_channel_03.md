
## goroutine / channel

* 引数に指定されたURLをhttp getで取得し、各URLのサイズを表示するプログラム

```
$ ./fetchall https://www.google.co.jp/ http://www.yahoo.co.jp/ https://github.com/
0.20s   19419 http://www.yahoo.co.jp/
0.38s   11912 https://www.google.co.jp/
1.60s   24816 https://github.com/
```
