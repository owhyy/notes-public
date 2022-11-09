# Predicates

#Databases #Programming #SICP

> #[[Functions|Function]] that checks whether something is of some type/kind:

- `(string? something)` is a Racket predicate, that checks if something is a string
- [[Clauses|LIKE]] is a [[Databases and Tables|SQL]] predicate, that checks if something matches some pattern/ _is like something_
- a predicate is also similar to a operator, but not quite like it:
  - `a = b` is an operator but not necessarily a predicate, because it answers the question _is `a` the **same thing as** `b`_, rather then _is `a` **like** `b`_ or _is `a` **of the same kind as** `b`_
