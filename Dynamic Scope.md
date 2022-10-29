# Dynamic Scope
#SML #Programming 
> Functions use the environment where the [[Functions|function]] is used
```sml
val x = 1
fun f y = x + y
val x = 3
```
* `f` will be a function that adds 3; further modification of `x` will also modify the behavior of `f`