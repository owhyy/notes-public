# Shadowing
#Programming #SML
+ `val a = 15`
+ here a's [[Variable Bindings|static environment]] is `int`, and its dynamic environment is `15`; 
+ `val b = a + 5`
+ b's static environment is `int`, dynamic is `20`;

+ now, if we do something like
+ `val a = 3` - this DOES NOT change `a`'s environments; it creates a new variable with a new dynamic environment
+ also, `b` does not change; it is bound to `20`, but it does not matter where it got that 20