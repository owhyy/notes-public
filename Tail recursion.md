# Tail recursion

#Programming #SICP #SML

> Position in which the operation called is the one producing the result of the whole [[qznn-recursion|recursive function]]

```scheme
(+ (first lon)
	(sum (rest lon)))
```

gets us this:
`(+ 1 (+ 2 (+ 3 (+ ... ` until `lon` is empty

in Tail recursion, every recursive call produces the result of the previous call

```scheme
(sum (rest lon)
(+ acc (first lon)))
```

will get us the result, when `lon` is empty, but will not push the `+` unto the stack

In [[Mutually recursive data|mutually recursive functions]], each recursive call must be in tail position.
