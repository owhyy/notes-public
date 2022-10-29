# Wildcards
#Databases 
> A wildcard is a character used to match some text. In SQL, these are some of them:
* The `%` wildcard, which is similar to `*` in Unix. It basically does the same thing: `%.com` and `*.com` would select the same stuff 
* Another wildcard is `_`, which is the same as `%` but only for 1 character
* The wildcard `[AB]%` will match all columns that start with A or B. This is called a set, but is not available in all DBMS.
* The `^` wildcard acts as a NOT
> It is best we avoid wildcards, because they will slow down our [[Queries|queries]]