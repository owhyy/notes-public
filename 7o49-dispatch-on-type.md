---
title: Dispatch on Type
created: 2022-09-11
keywords: [SICP, Programming]
---

# What?

- Design implementation where the [[qe97-generic-interface|generic interface]] calls the right method for a type using a [[Case expressions|case expression]].

## Pseudocode:

```
foo, bar, baz are types
f_foo(obj: foo), f_bar(obj: bar), f_baz(obj: baz) are functions for them
g(obj: any) is a generic interface that should call the method for foo, bar, baz:
define g(obj):
  switch type obj:
    case foo: f_foo(obj)
    case bar: f_bar(obj)
    case baz: f_baz(obj)
    ...
```

# Weaknesses

1. Adding a new type would require the [[qe97-generic-interface]] to add a new case to every existing case expression.
2. We must be careful to avoid name clashes, (since every new type will require a bunch of new functions, with similar names).
