# Data abstraction

#SICP #Programming #SML

> Separating the implementation from the usage, and creating [[Functions]] that operate on data regardless of how it's represented

# Example:

- A forest is a #[[Lists|list]] of trees, so we use `cons`, `car` and `cdr`;
- A [[Tree]], however, is implemented in terms of tree-related functions. Even if it's implemented in terms of `car` and `cdr`, we use `make-tree`, `datum` and `children`
