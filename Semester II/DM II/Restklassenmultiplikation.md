#### <font color = "orange">Entscheidungsdiagramm</font>

> [!HELP]
> ![[PXL_20241007_120801482 1.jpg]]

#### <font color = "orange">Wie man Restklassen multipliziert:</font>
$[a]$<sub>m</sub> $* x = [b]$<sub>m</sub>
$g$ ist nun der $ggT(a,b)$. Ist **$b$ durch $g$ teilbar**, **gibt es eine Lösung**. Diese wird dann errechnet, indem man den [[Erweiterter Euklid]] nutzt, um **t zu bestimmen**. 

Um schließlich **alle Lösungen** zu bestimmen, muss in folgende Gleichung eingesetzt werden:
$x = [(b/g)*t+j*(m/g)]$

>[!HINT]
>$j$ ist dabei eine Laufvariable, die von $0$ bis $(g-1)$  durchläuft.

Ist $t$ negativ, muss der **[[kanonische Repräsentant]]** der Restklasse gebildet werden. Dafür wird schlicht der Modulo $m$ auf $t$ addiert.

Ist $b$ **nicht** durch $g$ teilbar, gibt es **keine Lösung**.

#Restklassen #DMII