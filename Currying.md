# Currying
#SML #Programming 

> Transforming a [[Functions|function]] that takes multiple arguments into one that takes one argument and returns a function taking the next arguments and so on
```sml
val f = fn x => fn y => fn z => ...
val t = ((f 1) 2) 3
```

## Partial application
Since currying returns a function, we can do something like
```sml
val f = fn x y z => x + y + z
val t = f 1 2
```
Which means that `t` will be a function that takes a argument `z` and applies `f` (adds) it to `1` and `2`
* This is essentially *passing a function to another function*, however this will also create a new function that you can pass around, which makes it easier to [[Abstraction|abstract]] functions: you can create a curried general [[Higher-order procedures|higher-order procedure]], and use partial application to create new procedures based on it