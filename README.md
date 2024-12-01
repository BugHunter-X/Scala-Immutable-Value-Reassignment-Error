# Scala Immutable Value Reassignment Error

This example demonstrates a common error encountered in Scala programming: attempting to reassign an immutable value. In Scala, variables declared with `val` are immutable, meaning their values cannot be changed once assigned.

## Bug Demonstration

The `bug.scala` file showcases the issue. It initializes an immutable variable `x` with the value 10 and then attempts to reassign it to 20. This will result in a compilation error.

```scala
val x = 10
println(x)

x = 20 // This line causes the error
```

## Solution

The `bugSolution.scala` file provides the corrected code. To allow for reassignment, the variable should be declared with `var` instead of `val`.

```scala
var x = 10
println(x)

x = 20 // Now this works correctly
```