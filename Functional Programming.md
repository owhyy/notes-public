# Functional Programming vs OOP

#Programming #SML #OOP

# Functional Programming means:

1. no mutation
2. [[Higher-order procedures|functions are values(aka Higher-order functions)]]

- basically, a functional language should support:
  1.  immutable data
  2.  [[Function Closures]]
  3.  [[Functions#First class and Higher-order functions]]

# Functional vs OOP/DDP vs MP

- Functional and OOP are exactly opposite ways to look at the same things, so it's not a matter of _this is better than that_, but rather of _which one to use, depending on the way the code is going to grow_:
- [[unl2-data-dircted-programming]] and [[zd0v-message-passing]] is exactly the same as Functional vs OOP.

## Functional/[[unl2-data-dircted-programming|Data-Directed]]

> Creating new functions is faster, creating new types is slower

- Adding a new function means creating a new [[Case expressions|case expression]] (fast)
- Adding a new type means adding a new case for all of the case expressions (slow)

## OOP/[[zd0v-message-passing]]

> Creating new types is faster, creating new functions is slower

- Adding a new function means adding it to all of the classes (slow)
- Adding a new type means implementing all functions for it (fast)
