---
title: The Adapter Pattern
created: 2022-07-12
keywords: [Python, OOP, Programming]
---

# How?

Make our object look like the object that the class's constructor expects(has the same function names, variable names etc.), but implemented their own behavior.


# Why?

Used when we want to add functionality our object we initialize with isn't designed for.
For example, we have `Shape` class for which we want to implement a text class, but we want to reuse an already existing text view with functions. However, the names of the functions in `TextView` don't match those that `Shape` objects must have, so what we can do is create a `TextShape` that will [[Inheritance|inherit]] from `TextView` and define the methods that `Shape` expects.
