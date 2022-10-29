# Clauses
#Databases 
> A word specifying details about a [[Statements|statement]]
## ORDER BY
As we saw in [[Statements]], the `FROM` is a clause. It's kinda like it tells the statement what to do.  Some of them are optional, like the `ORDER BY` clause, while some are part of the statement.

> The `ORDER BY` clause has to be last in a `SELECT` statement
> The `ORDER BY` clause takes a [[Databases and Tables|column]] name (or more), by which it ascendingly (by default) sorts the statement. You can also specify the order by which to sort, with an `DESC` or `ASC` clause, after the column name

## WHERE
The `WHERE` clause works similar to an `if` expression. The syntax looks like
`SELECT ... FROM ... WHERE condition;`

> A cool thing involving operators is the `IN` operator:
`.... WHERE col_name IN (smth_1, smth_2, ...)`, which works like a `... WHERE col_name = smth_1 OR col_name = smth_2 OR col_name = smth_n...` but wayy less typing

In order to search for text patterns, we use the `LIKE` [[Predicates|predicate]]:
`SELECT ... FROM ... WHERE something LIKE some_pattern`

A pattern can include [[Wildcards|wildcards]]

## GROUP BY
[[Functions|Aggregate functions]] are cool if we want the number of [[Databases and Tables|rows]], but if we want a more specific search, like the number of rows of a specific vendor, we can use groups. 
In other words, `GROUP BY` groups rows based on a specific criteria, and then aggregate functions are calculated for each of the groups.
> The `GROUP BY` clause will automatically sort and split all rows, and return the groups of data based on the previous clauses

You cannot use `GROUP BY` with aliases

## HAVING
`HAVING` has the same function as `WHERE`, except it operates on groups instead of rows