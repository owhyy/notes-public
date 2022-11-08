---
title: Functional Programming vs OOP
created: 2022-10-30
keywords: [Programming, OOP]
---

# Functional Programming vs OOP

> Functional and OOP are exactly opposite ways to look at the same things, so it's not a matter of _this is better than that_, but rather of _which one to use, depending on the way the code is going to grow_:

> [[unl2-data-dircted-programming]] and [[zd0v-message-passing]] is exactly the same as [[ojgq-functional-programming]] vs [[g7tr-oop]].

## #[[ojgq-functional-programming]]/#[[unl2-data-dircted-programming|Data-Directed]]

> Creating new functions is faster, creating new types is slower

- Adding a new function means creating a new [[Case expressions|case expression]] (fast)
- Adding a new type means adding a new case for all of the case expressions (slow)

## #[[g7tr-oop]]/#[[zd0v-message-passing]]

> Creating new types is faster, creating new functions is slower

- Adding a new function means adding it to all of the classes (slow)
- Adding a new type means implementing all functions for it (fast)
