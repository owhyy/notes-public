---
title: Modular Design
created: 2022-07-26
keywords: [Programming, Software Architecture]
---

- A good module is a deep module: one that has powerful functionality but simple [[Interfaces]]. Microwave analogy: it's very complex inside, but has only a few simple buttons that controls it.
- Although this helps make code more obvious(especially if you use good names) and simpler to use, if the implementation is complex, code will still be [[84su-complexity|complex]]
- This goes against Clean Code advice of splitting long methods/classes into smaller ones. A class can be big, as long as its interface is small and obvious.

- Disadvantages of having a bunch of small classes and methods are that 1. there's a lot of boilerplate and 2. it is easier to work with a small class, but a lot of small classes that really do(or help do) the same thing add unnecessary complexity:

```java
FileInputStream fileStream = new FileInputStream(fileName);
BufferedInputStream bufferedStream = new BufferedInputStream(fileStream);
ObjectInputStream objectStream = new ObjectInputStream(bufferedStream);
```

You need to write all of this only to read from a file.

- One advantage I see to small classes, however, is that you can always make something like `function FileReader(fileName): {FileInputStream fileStream = new FileInputStream(fileName)...}`, and have no boilerplate and provide a simple interface at the same time. After all, simple interfaces will have a implementation that is more complex, so I'm not really sure why author didn't even mention this kind of solution?
