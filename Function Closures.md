# Function Closures
#Programming #SML #SICP 
## SML
> The pair (the function code and the environment that was current when we created the function)

1. the ability of functions to use free variables (variables defined outside the function)
```sml
val x = 1;      (* free variable *)
fun f y = x + y (* binds f to closure where x maps to 1 *)
val x = 3;      (* x is shadowed, f still uses x as 1 *)
```
2.  [[Let expressions]] and closure
```sml
val x = 1 (* x maps to 1 in the environment *)
fun f y = (* binds f to closure where x is 1 *)
	let 
		val x = y+1 (* creates new closure for x *)
	in
		fn z => x+y+z (* z binds to closure where x is y+1 *)
	end

f 4 (* will return a function that adds 9 to something *)
```

### Lexical scope and Dynamic scope
+ [[Lexical Scope]]
+ [[Dynamic Scope]]

### Closure Idioms
+ function composition: `fn x = f(g(x))` (*you've seen this already, included just for example*)
		- equivalent to `(f o g) x`; however, this is *right to left* (first apply `g(x)`, and then apply `f` on the result of `g(x)`)
		- `x |> g |> f` is equivalent to the above, but it is *left to right*
+ [[Currying]]

## Racket
> The ability to create [[Compound data]] from other [[Compound data]]: 
`(cons (cons 1 2) (cons 2 4)) -> a pair of pairs`

## OOP
In #OOP languages, closure is achieved via [[Class|classes]]:
- you can't have an array of arrays, but you can have an array of class objects that contain arrays as their fields
- this means that closure in racket is cooler
- I have wondered if there are languages that offer both, arrays and lists, but I doubt it's needed, as they are generally used for the same kinds of things, and lists are easier to use
