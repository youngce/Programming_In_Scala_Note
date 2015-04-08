# Learn to use the Scala interpreter
* [Scala Download](http://www.scala-lang.org/download/all.html)
* [Scala Install](http://www.scala-lang.org/download/install.html)

在安裝完Scala後，使用scala指令，可以呼叫出互動式的"shell"，如下
![](http://content.screencast.com/users/yangtsechung/folders/Jing/media/a05f767c-1b78-4464-8054-51f01ded38a0/00000029.png)

接著我們可以嘗試一些語法，如
```scala
scala> 1+2
```
輸出`res0: Int = 3`
* 計算值的變數名被自動生成或由使用者定義(res0意指result 0)
* 冒號（：）表示res0的類型

`resX`是可以被重覆使用的，如`res0 * 3` 將會輸出9

```scala
scala> res0 * 3
res1 * Int = 9
```

`println`函數可以印出字串，類似於JAVA中的`System.out.println`
######Example
```scala
scala> println("Hello, world!")
Hello, world!
```




