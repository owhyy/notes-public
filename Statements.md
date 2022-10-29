# Statements
#Databases 
> The simplest action you can do in a database
* A `SELECT` statement retrieves a column from a **[[Databases and Tables|column]]**. A `SELECT` statement is also called a [[Queries|query]].
* A `FROM` statement chooses the table from which to retrieve. This is also called a **[[Clauses|clause]]** for the `SELECT` statement.

  * It's easier to read code if you break it up, but you don't have to
 > Avoid using the * [[Wildcards|wildcard]] unless you really have to, cuz it's slow if you have a lot of columns

* The `DISTINCT` keyword is really cool, as it only selects unique values, but is applied to every single column, so if you have something like
* `SELECT DISTINCT col_name1, col_name2 FROM ...` this will select all columns that are distinct both, in `col_name1` and `col_name2`

### Comments
Comments are added with `-- some stuff`, `# some stuff` or `/* some stuff */` *(which has the same function as in C++)*