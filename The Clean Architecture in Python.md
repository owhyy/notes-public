#Python #Programming

- [Link to video](https://www.youtube.com/watch?v=DJtef410XaM)
- Main idea is to _separate the certain parts of a program_, and do so by _breaking it up into various small functions_, that _do a specific thing_: (in his example, the creation of the url is separated from the processing of data returned by creating a request on that url. There are [[Functions|no side-effects, every procedure takes some data and returns some data]]), and _have names that document what the function actually does_
- This simplifies testing (you can easily test every part of the code without #[[Dependency Injection]] or [[Mocking]])
