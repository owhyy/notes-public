# Joins
#Databases 

> A **join** joins some related tables, as if all the data were in the same one:

`SELECT name1_t1, name2_t1, name1_t2, name2_t2` <- data from two different tables
`FROM t1, t2` <- two different tables
`WHERE t1.some_id = t2.some_id;` <- join condition. This is what logically pairs the rows in the first table to the rows in the second.

### Inner Joins

The same can be achieved in a different syntax, even though technically they are both *inner joins*:
`SELECT name1_t1, name1_t2, name2_t2`
`FROM t1`
`INNER JOIN t2 ON t1.some_id = t2.some_id;`
Here, it will join ONLY the rows which have equal `some_id`s

### Self Joins

See [[Fields]] for table aliases.

*Self joins* are based on using the same table twice:
`SELECT ...`
`FROM` **`tab_name AS T1, tab_name AS T2`**
`WHERE T1.some_name = T2.some_name;`

### Outer Joins
  
 An *outer join*  only includes rows from one side or the other
`SELECT * FROM Tab1`
  **`LEFT`** `OUTER JOIN Tab2 ON Tab1.some_id = Tab2.some_id;` will join all of the rows which have equal `some_id`s and also the rows of `Tab1` which do not have `some_id` equal to `Tab2.some_id`.

![[left_join.png]]

`SELECT * FROM Tab1`
  **`RIGHT`** `OUTER JOIN Tab2 ON Tab1.some_id = Tab2.some_id;` will join all of the rows which have equal `some_id`s and also the rows of `Tab2` which do not have `some_id` equal to `Tab1.some_id`.
  
  ![[right_join.png]]
