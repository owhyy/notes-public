* Single element tuples must be written with a trailing comma (otherwise it's interpreted as an expression?)
- They are also unnamed dicts, where their meaning is given by the position of its items
- Tuple unpacking (actually *iterable* unpacking, since you can also unpack iterators): really useful feature, and is better, since you don't have to use indexes. Can be done in 2 ways
	- *paralel assignment: `a, b = (c, d)`*
	- prefixing with * (which unpacks all unassigned variables into a list); also works in function calls (args and kwargs)
		- can also be used to create lists and tuples easily from range functions. But I think `list(range(x))` is better, since it does not have to copy?
- Uses less memory than a list, because it can generate the bytecode for it in one operation, since it knows the size, since tuples are fixed length. Lists also have to be recopied if they preallocated size gets used up
- Tuples are immutable, but mutable variables inside a tuple (lists, for example) can still be modified: `([3,4], 2)[0].append(5)` will work, and modify the list. Use `hash(t)` if u need to check that everything is immutable
- [Why numbers should start at 0 by Djikstra](https://www.cs.utexas.edu/users/EWD/ewd08xx/EWD831.PDF)