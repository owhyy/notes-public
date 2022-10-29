---
title: Information Hiding
created: 2022-07-26
keywords: [Programming, Software Architecture]
---

> Making information impossible to acces or depend on from outside a module, and is not part of the [[Interfaces|Interface]]. Making information specific only to one module, and not letting other modules depend on the same things that the first module depends on

- Making information private isn't the same as hiding it if it can still be accessed through getters and setters, and if 2 modules depend on the same information

- Every time the same knowledge is used in multiple places, you create _information leakage_. Now, every time the information changes, you have to change it in all modules
- Solutions to this:
  - if modules are small -- merge them together inside one big module
  - extract the common information to a new module. Not sure how this works, thogh, since your other modules will still depend on one big module?
