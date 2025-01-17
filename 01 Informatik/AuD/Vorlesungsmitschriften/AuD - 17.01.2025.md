# <font color = "orange">AuD - 17.01.2025</font>
$n$: Eingabe $n$
Basisoperation: $+$
Best / Worst / Avg: gleich
Rekursionsgleichung, die die Ausführungshäufigkeit der Basisoeperationin Abhängigkeit von $n$ stellt.

$F(n) = {0\text{, wenn }n=0}$
$F(n) = {0\text{, wenn }n=1}$
$F(n) = {1+F(n-1)+F(n-2)}$
$= 1+1+F(n-2)+F(n-3)+1+F(n-3)+F(n-4)$
$= 1+2 +F(n-2)+2F(n-3)+F(n-4)$
$= 1+2+1+F(n-3)+F(n-4)+2(1+F(n-4)+F(n-5))$
$= 1+2F(n-5)+F(n-6)$
$= 1+2+3+F(n-3)+3F(n-4)+3F(n-5)+F(n-6)$
$= 1+2+4+8$
$= \sum = 2^n -1 \in \Theta (2^n)$
