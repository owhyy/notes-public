# `let` expressions

#Programming #SICP #SML

## Racket

- syntax: `(let bindings body)
- `let` vs `let*` vs `let-rec`

```scheme
(let ((a 3) 	  ; binding
	 (b (+ a 2))) ; binding
	 (+ a b)) 	  ; body
```

will not work, because **the body is evaluated first**, and `a`'s value is not known at binding; however,

```scheme
(let* ((a 3) 	   ; binding
	  (b (+ a 2))) ; binding
 	  (+ a b)) 	   ; body
```

will work, because it gets evaluated to:

```scheme
(let ((a 3))		 ; binding
  (let ((b (+ a 2))) ; binding INSIDE body
	 (+ a b)))       ; body of last let
```

here, `a` is replaced inside `b`'s body as well

- for the same reason, recursion won't work: the value of variable is known only inside the body, not in the binding

## SML

- syntax: `let b1 b2 ... bn in e end`
- evaluation/type-checking: value/value of `e` is value/value of `let` expression
- **available only inside the procedure**
