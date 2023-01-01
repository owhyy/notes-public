# Anonymous functions

#Programming #SICP #SML

> A #[[Functions|function]] that has no name

## [[2by8-scheme]]

- syntax: `(lambda (name) (...))`

* `(define (function x) (...))` is just syntactical sugar for `(define function (lambda (x) (...))`, because **in scheme, lambdas can be used for recursion**

## [[mo3z-sml]]

- syntax: `((fn name) => ...)`
- [ ] `fun name (x, y) = ...` is just syntactical sugar for `val name = fn (x, y) => ...`; combining the two, we get `fun name x = fn y => ... `; this is called [[Currying]]

## [[799a-javascript]]

- there's lambda functions: `const fun = value => value * 2`:
- and there's anonymous functions (yeah, they're not the same, although...): `const fun = (function someFuncition(value) {return value})` -- basically you can name it
