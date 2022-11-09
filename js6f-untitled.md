---
title: Why don't you want getters and setters?
created: 2022-07-22
keywords: [Python, OOP, Backend]
---

[Link to article](https://stupidpythonideas.blogspot.com/2015/01/why-dont-you-want-getters-and-setters.html?q=getters)

- Article says that the argument that getters and setters "for #[[Incapsulation]]" is bs in python, since 1. everything is public anyway and 2. it doesn't help encapuslation in any way (`x.age = 3` and `x.set_age(3)` mean the same and expose the `age` variable in the same way.
- A use for getters and setters is computed properties. However, here to, computing properties is a implementation detail, not part of the [[Interfaces|interface]]. The solution is to use `@property` to represent the attribute.
- For read-only attributes, again `@property`
