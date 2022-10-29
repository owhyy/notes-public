# Dependențe funcționale
#Databases 

> O dependență funcțională $X \rightarrow Y$ înseamnă că dacă știm $X$ putem afla $Y$

O dependență funcțională nu e o funcție (in the sense that we plug a number and get a result), ci  o operație de căutare

|a|b|
|---|---|
|1| 2|
|2| 3|
|3| 9|

 + if a=2, b=3; the same way a [[Functions]] in math always gives the same result on the same inputs:
 $x=5, y=2x$ then, $y$ is always going to be $10$
 + `if t1.x=t2.x and t1.y=t2.y` then it is a functional dependency; 
 + `if t1.x != t2.x` then it is a functinal dependency;
 + otherwise, not:

|a|b|
|---|---|
|1| 2|
|**2**| **3**|
|**2**| **3**| 
is a funtional dependency, while 

|a|b|
|---|---|
|1| 2|
|**2**|**3**|
|**2**|**9**|
is not.

## Tipuri de dependețe funcționale
+ trivial: $X \rightarrow X$ ($X$ se determină pe sine însuși); același lucru ca $Y \subseteq X, \ X \rightarrow Y$; ex: dacă $X=ab$ și $Y=b$, atunci $Y \subseteq X$ și deci avem o dependență trivială;
+ non-trivial: $X \rightarrow Y, X \cap Y = \varnothing$ ($X$ și $Y$ nu au elemente comune)
