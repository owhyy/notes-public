---
title: TDD
created: 2022-09-01
keywords: [Programming, Software Architecture]
---

# How do I?

0. Write a to-do of all(that you can think of in that moment) the stuff that you want your program to do
1. Write a test that will cross off a item on your to-do
2. Make the test work, then make it pass, doing whatever is necessary for it to pass
3. Refactor and clean duplication

# Obvious Implementation, Fake it and Triangulation

- If coming up with a solution that will make the code run is obvious -- do it
- Otherwise make your functions return constants, and then gradually replace them with real code
- When completely unsure of how to refactor, try doing 2 test cases of the same thing to come up with a solution (suppose we want to test for addition, we would do something like `assert 1 + 1 = 2` and `assert 1 + 2 = 3`)

# Never interrupt an interruption

- [[Mocking]]#
