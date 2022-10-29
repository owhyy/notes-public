# Pattern Matching
#Programming #SML
+ every [[Function Bindings|function]] takes one argument, so there's no need for `fun x(v:t1*t2*tn)=e`; we can do just fine with `fun x(v1, v2, v3)=e`
+ type inference: type of `x` gets deduced from the function itself