# Attribute closure
#Databases 
> used to find [[Keys#Candidate Key|Candidate Keys]] in a [[Databases and Tables|relation]]
+ $x^+$ - attribute closure of $x$; contains all attributes determined by $x$;
ex: let $R(A,B,C,D,E)$ and $A$ be a [[Dependențe funcționale|functional dependency]] such that $A \rightarrow ABCDE$, then $A^+=\{A,B,C,D,E\}$
+ every FD in the set must be determined by something ($B$ can be in a set only if there's some FD $x$, such that $x \rightarrow B$)
+ 