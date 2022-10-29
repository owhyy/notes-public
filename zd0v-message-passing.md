---
title: Message Passing
created: 2022-09-13
keywords: [Programming, SICP]
---

# What?

- Smart procedures: each procedure returns a interface accepting a message, where every method is implemented for the message.

## Pseudocode

```
foo is type
i is function(n: foo), that will act as foo's interface, providing access to its functions:
  return lambda message:
    switch message:
      case sum: return lambda x: n + x:
      case sub: return lambda x: n - x
    ...

create a object
obj=f(5)
obj is now a interface. We can call foo's sum on 13 if we want,
by calling 'sum on the interface to get the sum method defined for foo:
apply(apply(obj, 'sum), 8) -> 13

```

# Why?

- Easier to encapsulate data than [[unl2-data-dircted-programming]]: _want to create a new object? just create a new interface; no need to modify existing ones_
