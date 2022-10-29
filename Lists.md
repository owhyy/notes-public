# Lists

#Programming #SML #Java #SICP

## SML

- non-fixed length
- [[One-of types]]
- syntax: `[e1,...,en]` or `[]`
- `empty?` <=> `null`
- type-checking: `t list`; **all elements `e` must have same type**
- evaluating: a list is a value of the above type
- cons: `(cons e1 e2)` in Racket <=> `e1 :: e2`;
- access: `hd` <=> `first`, `tl` <=> `last` (built-in) or [[Case expressions]] (better way, see [[Polymorphic Datatypes]])

- Lists are essentially a [[Polymorphic Datatypes]], in which there are 2 cases: `null` or `t list`, where `t` is the type, which has to be the same everywhere

## Java

- **lists can be synchorinzed or unsynchronized:**
- synchronized means only one [[Threading]] can perform actions on list, unsynchronized means that more threads can; `Vector` is the same thing as `ArrayList` except it is synchronized

## Scheme

- lists are just a chain of [[Pairs]]: `(list a b c d e)` <=> `(cons a (cons b (cons c (cons d (cons e nill)))))`
- lists(sequences) serve as ground for [[Stream|processing modules]]

## Python

- lists are _mutable_ (changing elements of a list will change it everywhere the list is used)
- reassigning lists however, won't mutate it, as it's going to act like a copy (not sure how this works)
- lists elements can have different types (unlike SML)
