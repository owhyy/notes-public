---
title: CSS
created: 2022-07-09
keywords: [Backend]
---

- Selector is what you apply it to ([[HTML & CSS|element, id, class]])
- In 99% of cases, use class selectors

# Selector combinations
- Can combine selectors with `.`: `h1.someclass` will select all `h1` headings containing the `someclass` class.
- Can select stuff inside other selectors with space: `div p` selects all paragraphs inside a `div`s.
- Can combine selectors with the same value using `,`, to avoid duplication: `h1, h2` will set the same properties to all `h1` and `h2`s

# Overriding
> id > class > element
