#### <font color = "orange">Wieso nutzen wir das?</font>
Um bspw [[El Gamal]] zu knacken, ist eine bestimmte Formel notwendig, der **[[dlog]]**. Das ist der **Diskrete Logarithmus**. 

#### <font color = "orange">Funktionsweise</font>
>[!FORMELN]
>**Formeln für den dlog:**
>$lsg = q*s+r$
>$s = ⌈√p-1⌉$
>**B.S.:** $y*g$<sup>-r</sup> mod $p$
>**G.S.:** $g$<sup>q*s</sup> mod $p$

Zunächst wird hierbei die Tabelle aufgebaut. Gegeben wird normalerweise $g$, sowie $y$.
In Verbindung mit  [[El Gamal]] entspricht $y$ allerdings dem *private key*. 

Die Baby-Step-Tabelle muss komplett gefüllt werden. Anschließend wird die Giant-Step-Tabelle nach und nach aufgebaut, wobei laufend überprüft wird, ob eine der Zahlen in dieser Tabelle auch in der Baby-Steps-Tabelle vorkommt.
Falls ja, wird das dazugehörige $q$ und $r$ in die **$lsg$-Formel** eingesetzt und so die Lösung errechnet.

>[!Example]
>$p = 19$ , $g = 14$ , $g$<sup>-1</sup>$= 15$
>$g$<sup>a</sup> mod $p= x = 3$
>**Dann gilt:** $dlog$<sub>14</sub><sup>(3)</sup> mod $19 = a$
>
>$s = ⌈√19-1⌉ = ⌈√18⌉ = ⌈4,24⌉ = 5$
>
>**Giant Step (q)**| $0$ | $1$ | $2$ | $3$ | $4$
>----|--|--|--|--|--
>$14$<sup>q*5</sup> mod $19$ | $1$ |<font color = "red">10</font> | $5$ | $12$ | $6$
>---------------|--|--|--|--|--
>**Baby Step (r)**| $0$ | $1$ | $2$ | $3$ | $4$
>$3*15$<sup>r</sup> mod $19$ | $3$ | $4$ | <font color = "red">10</font> 
>
>Somit ist $q = 1$ und $r = 2$. Es ergibt sich: $x = g*s+r=1*5+2=7$
>Damit ist $g$<sup>x</sup> mod $p = 14$<sup>7</sup> mod $19 = 3$


#dlog #crypto #DMII