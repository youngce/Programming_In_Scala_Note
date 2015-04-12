# Define some variables
Scala有兩種變數類型`var` and `val`

`val`一旦初始化，將無法重新賦值；`var`則可在生命週期範圍內任意地重新賦值。

```scala
// Here's val definetion
scala> val msg = "Hello, world!"
msg: String = Hello, world!
```
這個例子說明了Scala編譯器可以推斷類型，這樣往往是最好的做法法，而不需要顯式類型的註解。但有時候明確指定類型保證Scala編譯器推斷的類型是你想要的，而且增加代碼的可讀性。

在Scala中，可以在變數名之後加上類型，並以冒別區隔，如
```scala
val msg2: String = "Hello again, world!"
msg2: String = Hello again, world!
```
讓我們回到msg, 它是一個`val`而不是`var`，來看看如果重新賦值給它會如何，
```scala
msg = "Goodbye cruel world!"
```
```
<console>:8: error: reassignment to val
       msg = "Goodbye cruel world!"
           ^
```
如果你想對變數重新賦值，應該使用`var`,
```scala
 scala> var greeting = "Hello, world!"
 greeting: String = Hello, world!

 scala> greeting = "Leave me alone, world!"
 greeting: String = Leave me alone, world!
```
