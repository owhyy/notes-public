---
title: Database Indexing
created: 2022-08-18
keywords: [Databases, Programming, Backend]
---

> A way of sorting records of fields in a #[[Databases and Tables|database]], in order to increase search performance by allowing [[qphl-binary-search]] to be performed.

- Excessive indexing of a database will take up a lot of space. This is why you should index only records that you know search will be performed on.
- Also, indexing on a field that is no unique will decrease the effectivity of the search, so it should be avoided as well.
