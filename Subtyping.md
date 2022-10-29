# Subtyping
#Programming #SML #OOP

> If `e` has type `t1`, and `t1` is a subtype of `t2`, then `e` **also has type `t2`**
- A way to allow you to *forget* fields:
something like `fun distToOrigin (p:{x:real, y:real})` will only accept a [[Records]] of type `{x:real, y:real}`, like. Subtyping allows us to anything, as long as it has the 2 `real` parameters 
## Subtyping rules
1. Width subtyping - you can have a subtype have the fields of a supertype + some fields specific only to the subtype
2. Permutation subtyping - the order in which the fields are specified does not matter
3. Transitivity - if `t1` is a subtype of `t2` and `t2` of `t3`, `t1` is a subtype of `t3` (all subtypes of a supertype subtype are also subtypes of the supertype)
4. Reflexivity - every type is a subtype of itself
5. You cannot acces the fields of a subtype when using a supertype:
   ```sml
	A: {a:real, b:real}
	B: {a:real, b:real, c:real} (* B is subtype of A *)

	val x = {a=3, b=5} (* type A *)
	x.c   (* error, type A doesn't know about type c of its subtype*)

	(* it works the same way with functions *)
	fun funOnA(f: {a: real, b:real} -> {a:real, b:real}, 
			   p:{a:real, b:real}) =
		f p
	end
	
	(* expects B, which has c field *)
	fun funExpectsB p = if p.c = 5 ... (* error: is called with an A *)
	val y = funOnA(funExpectsB, x)

	(* but you can assume less *)
	fun expectsLess p = {x = ~p.a, b=10, c=15} (* will work, since we're creating a new object, and all we only access A's fields *) 
	```
7. Subtyping on [[Functions]] is *covariant*: if type `ta` is a subtype of `tb`, then a function `t -> ta` is a subtype of `t -> tb` (a function that expects a superclass can return more than just the superclass as long as it was called with an argument that is a subtype of that superclass)

- In OOP, subtyping is achieved via [[Inheritance]]