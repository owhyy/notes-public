# Keys
#Databases 
## Super Key
+ tuple or set of tuples that uniquely identifies a tuple;
+ $2^n-1$ maximum keys (in arbitrary table);
+ in the subset $\{A,B,C,D\}$, if $A$ is a super key, then so is every combination that includes $A$: $\{A,B\}, \ \{A,C\}, \ \{A,D\} \  \dots$, și invers, dacă $\{B,C,D\}$ is not a super key, then neither is any of the subset;
+ in a [[Attribute closure]], a super key is a closure set that contains all of a relation's [[Dependențe funcționale|functional dependencies]];

## Candidate Key
+ super key where [[Proper Subset]] is not a super key: for $\{A,B,C\}$, the proper subsets are $\{A,B\}, \ \{A,C\}, \ \{B,C\}, \ \{A\}, \ \{B\}, \ \{C\}$, so if any of those keys are super keys to the relation, $\{A,B,C\}$ is not a candidate key; **minimal super key**;
+ in a [[Attribute closure]], is the smallest super key which has no proper subsets;

## Primary Key
+ one of the candidate key where values are not null;