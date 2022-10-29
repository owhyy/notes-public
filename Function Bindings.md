# Function Bindings
#Programming #SML
> The act of creating a function
+ syntax:
`fun x0 (x1:t1, ..., xn:tn) = e` ([[Variable Bindings|something = something else]])
+ type-checking: binding every `x1, ..., xn` in body of `e` to their type `t`; type of `x0` is `t1*...*tn->t*`, where `t` is the type of `e`
+ evaluating: a [[Functions|function]] is a value
+ calling: `f0(x1,...,xn)`