# Data abstraction
#SICP #Programming #SML 

> Separating the implementation from the usage, and creating [[Functions]] that operate on data regardless of how it's represented

* For [[Tree]]: a forest is a [[Lists|list]] of trees, so we use `cons`, `car` and `cdr`; 
* A [[Tree]], however, is a tree. It has [[Node|nodes]] and leaves, so we don't use `car` and `cdr` (event though it is implemented in terms of a list, we don't care about that; we shouldn't care about how a tree is implemented), but `make-tree`, `datum` and `children`