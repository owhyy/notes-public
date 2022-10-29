# Graphs
#SICP #Programming 
Just like an [[Mutually recursive data|arbitrary errity tree]], but
+ you can go back to the previous node and nodes
+ can have multiple nodes going to a single node

```scheme
(define HS2 (shared ((-0- (make-house "A" (list (make-house "B" -0-)))))
		(list -0-)))
```