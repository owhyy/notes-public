# Variable Bindings

#Programming #SICP

> #[[mo3z-sml]] way to create a variable

- binding: something = something else: [[Variable Bindings]]#, [[Function Bindings]]#, [[Datatype Bindings]]#, [[Options]]#
- **static**/**dynamic environment** - **type**/**values** of preceding bindings

Example:
`val x = e;`

- type-check: **type** of `x` is type of `e`
- evaluation: **value** of `x`is value of `e`
- in ML bindings are _immutable_; you can't reassign `val x = 19` to `val x = 21`; in this case the second `x` [[Shadowing|shadows]] the first one
