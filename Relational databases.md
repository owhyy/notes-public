# Relational databases
#Databases 

> A *relational database* is a [[Databases and Tables|database]] in which every concept has a specific table.
 
For example, if we need a table containing data about some *Products* and the *Vendors* of the products. 

Now, if we have a *Vendor* that produces multiple *Products*, this means that we need to copy the information about that *Vendor* across every *Product*.

This is not a problem if information about the *Vendor* is short and concise, but if there are things like the Name, Date of Birth, Place of Living, State etc. we can already see how much *time* and *space* we would need to waste. Now, this is still not critical for 2-3 *Products* of the same *Vendor*, but if we have 100 of them, we're kinda fucked, because we need to copy the same exact things 100 times.
And, even then, suppose the *Vendor* changed its name. Then, we need to change the name on 100 tables...

This is where **relational databases** shine. You create a table for *Vendors*, a table for *Products*, and in the *Products* table you include only an **vendor ID**, which in the *Vendors* you declare as *primary key*. This allows you to access vendor-related columns from within *Products*, and this:
* needs less repeating
* does not need modifying every single Product table, if something about the Vendor changes
* data is consistent (less prone to human errors)