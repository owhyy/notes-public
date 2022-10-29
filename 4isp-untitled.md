---
title: Composition Over Inheritance
created: 2022-07-11
keywords: [Python, OOP, Programming]
---

# Why?

The problem with [[Inheritance]] is that oftentimes we need to implement a bunch of specialized behaviors, which leads to a bunch of subclasses. Suppose we have a simple class hierarchy:

```python
class Logger(object) # will be base class
class SocketLogger(Logger) # some class inheriting
class ...(Logger)
```

If we now want to add some new behavior, like filtering, we'll define a class

```python
class FilteredLogger(Logger) # class implementing filtering behavior
```

But here is where the problem lays. If we want to implement filtering to `SocketLogger` and other `Logger` derivated classes, we need to create new classes for every implementation. (*explosion of subclasses*)
