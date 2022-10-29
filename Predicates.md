# Predicates
#Databases #Programming #SICP 
> The kind of thing that checks whether something is of some type/kind:
* `(string? something)` is a Racket predicate, that checks if something is a string
* [[Clauses|LIKE]] is a [[Databases and Tables|SQL]] predicate, that checks if something matches some pattern/ *is like something*
* a predicate is also similar to a operator, but not quite like it:
	* `a = b` is an operator but not necessarily a predicate, because it answers the question *is `a` the **same thing as** `b`*, rather then *is `a` **like** `b`* or *is `a` **of the same kind as** `b`*