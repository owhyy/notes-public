# Queries
#Databases 

As mentioned in [[Statements]], a query is (generally) a `SELECT` statement.
A **subquery** is a query inside a query, and is used when you need to access a column of a table **based on the results of another query**

`SELECT name1`
`FROM tab1`
`WHERE name2 IN (SELECT name2 FROM tab2 WHERE condition)`
is an example of a subquery, which will retrieve `name1` from all of the columns in which the condition is true for `name2`

> Subqueries can only retreieve a single column

Even though subqueries are cool, it is better to use [[Joins]]