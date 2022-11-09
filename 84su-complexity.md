---
title: Complexity
created: 2022-07-25
keywords: [Programming, Software Architecture]
---

> Anything that makes code hard to modify and understand

# How to tell if something is complex?

- If it's hard to change:
  - Code has a lot of dependencies
  - Not sure what you have to change to complete a task (worst)
- If it's hard to understand
  **Sometimes code that requires more lines of code is simpler to understand**
- What causes complexity
  - Code being dependent on other code. If code has a lot of dependencies, implementing new features is hard, because you need to also modify the code on which it depends -> exponential raise of problems
  - Code is too general (obscure): bad variable names (too general), bad documentation, inconsistency
- How to reduce complexity
- [[nr4v-modular-design]]#
- Minimize dependencies
- If there needs to be a specific order on functions (not really a good thing, but sometimes unavoidable), document this in the [[Interfaces]]
- [[pmgf-information-hiding]]#
- [[no7r-red-flags-in-software-design]]#
