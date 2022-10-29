#Python #Programming
- [Link to video](https://www.youtube.com/watch?v=DJtef410XaM)
- Main idea is to *separate the certain parts of a program*, and do so by *breaking it up into various small functions*, that *do a specific thing*: (in his example, the creation of the url is separated from the processing of data returned by creating a request on that url. There are [[Functions|no side-effects, every procedure takes some data and returns some data]]), and *have names that document what the function actually does*
- This simplifies testing (you can easily test every part of the code without [[Dependency Injection]] or [[Mocking]])
