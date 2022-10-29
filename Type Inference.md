# Type Inference
#Programming #SML
> Trying to give every binding/expression a type, such that [[Type-checking]] succeeds or fails (if no solution exists)

+ a [[Datatype Bindings|type]] like `'a list * 'a list -> 'a list` is more general than `string list * string list -> string list` if `'a` can be replaced by more than 1 type; in this case, `'a` 's type is `string`, but it can be replaced with any other type, under the condition the every one of the 3 types are the same
+ but it is less general than something like `int list * string list -> int list`, because here we can only use the specified types, so `'a` can only replace `int list * string list` and `int list`
### How it happens
1. Top to bottom (if you want to use a [[Functions|method]] inside another method, you need to define it above, so it's in the environment)
2. Collect the constrains: function argument types, return types, if-then-else branch types and so on. If something doesn't match (result of the `if` branches differ, for example), throw errors
3. For the unconstrained types (or [[Parametric polymorphism]]) set type variables `'a`, `'b` ...