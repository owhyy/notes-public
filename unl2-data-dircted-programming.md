---
title: Data-Directed Programming
created: 2022-09-11
keywords: [SICP, Programming]
---

# What?

- **Same principle as calling the function iself instead of a `switch` statement**: Storing every data type and function for it in a table, then just look it up based on the type of the object:

## Pseudocode:

Our table can be thought of as a dict where the key is the type and the values -- functions defined for it.

```
foo, bar are types
f_foo(obj: foo), f_bar(obj: bar) are functions
g is a generic interface g(obj: any)

# first put functions into table
put(foo, f_foo, f)
put(bar, f_bar, f)

# then we can apply the function
define g(obj: any):
  type=table.get(foo)
  function=type.get_func(f)
  f(obj)
```

# Why?

- Solves weaknesses of #[[7o49-dispatch-on-type]]: names don't matter, only name of generic function;
- Easier to define procedures than [[zd0v-message-passing]]: _want to implement a new procedure? Just add it to the table._
