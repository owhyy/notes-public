# Fields
#Databases 
> The same as a [[Databases and Tables|column]], except it's used when you refer to one that's been modified in some way.
* For example, the stuff returned from `SELECT col_name FROM tab_name` is referred to as columns, while `SELECT '(' + col_name + ')' FROM tab_name` - as a field.
* Some DBMS include the padding spaces, so we use the `RTRIM()` or `LTRIM()` [[Functions|functions]] to get rid of them.
* A column can be aliased using the `AS` keyword. This makes it so we can use the field just as if it were a regular column.

> Even though `AS` is optional, it is considered best practice to always use it with fields 

A table name can also be aliased:
```sql
SELECT ...
FROM Tab1 AS T1, Tab2 AS T2
WHERE T1.some_id = T2.some_id
```
