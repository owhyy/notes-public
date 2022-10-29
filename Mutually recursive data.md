# Mutually recursive data
#SICP #Programming 

An **arbitrary errity tree** is a mutually recursive tree. It's just like a *binary tree*, but can have more than 2 branches (can grow in width)

The data definition includes the object's definition and a (listof the element)

Template for mutually recursive data (an arbitrary errity tree), with local:

```scheme
(define (fn-for-x x0)
	(local [(define (fn-for-x x)
		(... (name-x x) (something-else-x x) ** (fn-for--lox (subs-x x))))
	(define (fn-for--lox lox)
		(cond [(empty? lox) ...]
			[else
			(... (fn-for-x (first lox)
	(fn-for-lox (rest lox)))])]
 (fn-for-x x0)
 ```