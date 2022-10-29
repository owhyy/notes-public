# Records
#Programming #SML
+ [[Each-of types]], where every component is a named field:
+ syntax: `{foo = e1, bar = e2}`
+ type checking: `{foo : int, bar : int*bool, baz : bool*int}`
+ accessed by name: `#foo e` or by a [[Case expressions]]
+ [[Tuples|Tuples]] are records, where the fields are named `1, 2 ... n`