# Anonymous functions
#Programming #SICP #SML
> A [[Functions|function]] that has no name
## Scheme
* syntax: `(lambda (name) (...))`
+ `(define (function x) (...))` is just syntactical sugar for `(define function (lambda (x) (...))`, because **in scheme, lambdas can be used for recursion**

## SML 
+ syntax: `((fn name) => ...)`
+ [ ] `fun name (x, y) = ...` is just syntactical sugar for `val name = fn (x, y) => ...`; combining the two, we get `fun name x = fn y => ... `; this is called [[Currying]]