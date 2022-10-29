# Lexical Scope
#SML #Programming 
> Functions use the environment where the [[Functions|function]] is defined
```sml
val x = 1
fun f y = x + y
val x = 3
```
* `f` will always be a function that adds 1, no matter where it's called, because the value of `x` when `f` was defined was 1

This is good, because
*  we can rename variables without worrying about collateral effects
* functions can be type-checked where they are defined, rather than where they are used
* you don't have to worry about what you're naming your variables when passing functions