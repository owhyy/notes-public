---
title: SML Lists
created: 2022-10-30
keywords: [SML, Programming]
---

- non-fixed length
- [[One-of types]]
- type-checking: `t list`; **all elements `e` must have same type**
- evaluating: a list is a value of the above type
- created: `e1 :: e2`;
- access: `hd`, `tl` (built-in). [[Case expressions]] (better way, see [[Polymorphic Datatypes]])

> #[[mo3z-sml]] #[[Lists]] are essentially a [[Polymorphic Datatypes]], in which there are 2 cases: `null` or `t list`, where `t` is the type, which has to be the same everywhere
