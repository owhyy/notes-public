# Variable Bindings
#Programming #SICP

+ binding: something = something else: [[Variable Bindings]], [[Function Bindings]], [[Datatype Bindings]], [[Options]]
+ **static**/**dynamic environment** - **type**/**values** of preceding bindings

Example: 
`val x = e;`

+ type-check: **type** of `x` is type of `e` 
+ evaluation: **value** of `x`is value of `e`
+ in ML bindings are *immutable*; you can't reassign `val x = 19` to `val x = 21`; in this case the second `x` [[Shadowing|shadows]] the first one