---
title: C#
created: 2023-01-08
keywords: [Programming, Programming Languages]
---

> #[[g7tr-oop]] programming language, which started out as basically [[fqah-java]] but by Microsoft

# Modifiers

- `out` -- operation similar to tuple unpacking in [[ubm8-python]]. However, what differs is that, while tuple unpacking in python will set the first variable to the first value, in C# it's reversed, where the last variable will have the last element:

In python:
`x, *y = ('foo', 'bar', 'baz')` -- `x` is `'foo'`, `y` is `['bar', 'baz']`
`Split ("foo bar baz", out a, out b)` -- `a` is `"foo bar"`, `b` is `"baz"`

- `in` -- rough equivallent to `const static &` in [[l7p6-c]]: pass-by-reference, but don't copy and don't allow modification. I wonder what's the difference between this and `ref readonly`

- `params` -- kinda like `args` in Python, and the elipsis operator in [[2by8-scheme]]: allows any number of arguments of a specified type

# Target-Typed new Expressions

- really cool feature: in order to avoid duplicating code such as `Package.CustomClass x = new Package.CustomClass("foobar")` ca be written only as `Package.CustomClass x = new ("foobar")`

# Null-Coalescing Operator

- `??` operator, same as `or` assignment in python:

```csharp
string s1 = null;
string s2 = s1 ?? "foobar";  // s2 is "foobar"
```

Is the same as
`x = None or '1'`

# Null-Coalescing Assignment

- `foo ??= bar`: `if (foo == null) foo = bar;`

# Null-Conditional Operator

- `foo?.ToString();` -- cool, same as `foo == null? null : sb.ToString();`
- we can also set types to accept null, by appending `?` at the end: `int?`
