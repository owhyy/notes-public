# Iterative processes
#Programming #SICP #SML 
> A algorithm in which the results are computed and calculated based on the modification of a variable.

Structure of an iterative process: 
`(f (modify var) (get-closer-to-endcase))`
Memory is not used to keep track of the operations, as it happens in [[Recursive processes]] because the result is ready when the base-case is reached

Because of the nature of iterative algorithms, the (natural) way in which they are used with [[Lists#Scheme|consing to a list]], the result is actually in reverse order