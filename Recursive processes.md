# Recursive processes
#SICP #Programming #SML 
> Algorithms in which the result is computed based on a [[Tail recursion|tail]] of operations that gets evaluated when the base-case is reached.

Structure of an recursive process:
`(get-closer-to-result (f (get-closer-to-endcase))`
Memory is used to keep track of `get-closer-to-result` calls that get built up with each `f` call, which is different from [[Iterative processes]]