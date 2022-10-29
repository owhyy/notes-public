---
title: Red Flags in Software Design
created: 2022-07-26
keywords: [Programming, Software Architecture]
---

1. Shallow [[nr4v-modular-design|modules]]: complicated [[Interfaces]] (a lot of functions to call)
2. Information leakage: same knowledge is used in multiple places. (not sure what this means)
3. Pass-Through Methods: functions that do nothing but call another function: `function pass_thru(x): {return other_function(x);}`
4. BIG RED FLAG: Information leakage
