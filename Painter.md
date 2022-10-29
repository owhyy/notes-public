# Painter
#SICP 

* `painter` is the element that draws an image on a frame
* You can combine `painter`s, so you can draw the images `beside`, `below` etc
* Exploits [[Function Closures]]: a the procedures take `painter` as their arguments, and produce a new `painter`
* We [[Abstraction|abstract]] patterns by implementing them as Scheme procedures (not as a different kind of data), so we can use them with a lot of different images without having to duplicate code
* We can [[Abstraction|abstract]] the procedures, to create new procedures that also take procedures as arguments and create new painter operations ([[Higher-order procedures]])
* A frame has 3 vectors: origin (offset of origin from some origin in the plane) and 2 edge vectors (offset of frame corners from its origin); perpendicular edges -> square frame; otherwise -> parallelogram-like frame
* The coordinates of the vectors are numbers between $(-1; 1)$
* In order to scale an image to fit a frame, we map the $x$ and $y$ coordinates of the image to the vector sum of 




