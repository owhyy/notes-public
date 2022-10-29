# Reguli de inferență. Axiomele lui Armstrong
#Databases 
+ reflexivitatea: [[Dependențe funcționale#Tipuri de dependețe funcționale|dependență funcțională trivială]] ($X\rightarrow X$)
+ tranzitivitatea: dacă $X\rightarrow Y\  \& \ Y\rightarrow Z$ atunci $X\rightarrow Z$
+ incrementarea/augumentarea: dacă $X\rightarrow Y$ atunci $XA \rightarrow YA$; reflexivitatea;
+ aditivitatea/uniunea: dacă $X \rightarrow Y\ \& \ X\rightarrow Z$ atunci $X\rightarrow YZ$ (unești 2 tupluri)
+ proiectivitatea/decompoziția: dacă $X\rightarrow YZ$ atunci $X \rightarrow Y\ \& \ X\rightarrow Z$ (inversul la uniune)
+ pseudotranzitivitatea: dacă $X \rightarrow Y\ \& \ YZ\rightarrow A$, atunci $XZ \rightarrow A$
+ compoziția(nu e in teorie): dacă $X \rightarrow Y\ \& \ A\rightarrow B$ atunci $XA \rightarrow YB$