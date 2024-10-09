#### <font color = "orange">Was ist der Miller-Rabin-Test?</font>
Der Miller-Rabin-Test löst ein Problem mit dem [[Fermat-Test]], bei dem Zahlen als falsch positiv ausgegeben wurden. Der Test war dabei nicht in der Lage, diese zu korrigieren bzw als keine Primzahl zu erkennen.

>[!INFO]
>**Step-By-Step-Anleitung**
>**1.** Wähle eine Zahl $a$, die größer als $1$, aber kleiner als $n$ ist.
>**2.** Ist der ggT von $a$ und $n$ *nicht* $1$, dann ist ***n keine Primzahl***
>**3.** $n-1$ wird gleich $2$<sup>r</sup>$* s$ mod $n$ gesetzt.
>**4.** $s$ ist dabei zunächst $n$. $r$ ist dabei $0$.
>**5.** $n / 2$ ist nun $s$. $r$ wird um $1$ erhöht.
>**6.** Dieser Schritt wird **iterativ** wiederholt, bis $n$ **nicht mehr** durch $2$ geteilt werden kann. Bei jeder Iteration wird $r$ wieder um $1$ erhöht.
>**7.** Nun wird für jedes $r$ durchlaufen: $a$<sup>2<sup>r</sup> *s</sup> mod $n$. $r$ ist dabei zunächst $0$, dann $1$, bis $r$ erreicht wurde.
>**8.** Die Zahlen der Menge $X$, die herauskommt, werden überprüft. Sind alle Zahlen $1$ oder ist $1$ wenigstens einmal an **spätestens** vorletzten Stelle vertreten, so ist die Zahl **wahrscheinlich** eine Primzahl.

**Beispiel:**
*Prüfen Sie mithilfe des Miller-Rabin-Algorithmus, ob $n = 89$ eine Primzahl ist. Nutzen Sie hierfür die Basis $a = 5$. 
**Hinweis:** Sie dürfen annehmen, dass der ggT$(89,5) = 1$ ist.*

$n-1 = 88$. Daher gilt: $88 = 2$<sup>0</sup> $* 88$. 
1. $88 = 2$<sup>0</sup> $*88 = 2$<sup>1</sup> $* 44 = 2$<sup>2</sup> $* 22 = 2$<sup>3</sup> $* 11$
2. $r = 3$.
3. $5$<sup>2<sup>0</sup>* 11</sup> mod $89 = 55$
4. $5$<sup>2<sup>1</sup>*11</sup> mod $89 = 5$<sup>2</sup> mod $89 = 88$
5. $5$<sup>2<sup>2</sup>*11</sup> mod $89 = 25$<sup>2</sup> mod $89 = 1$
6. $5$<sup>2<sup>3</sup>*11</sup> mod $89 = 9$<sup>2</sup> mod $89 =1$
Daher ist die Menge $x =$ {$55,88,1,1$}
Es ist erkennbar, dass eine $1$ an vorletzter Stelle von $x$ steht, daher ist $n$ **wahrscheinlich** eine Primzahl.

>[!Tip]
>Die Wahrscheinlichkeit, dass $n$ *keine* Primzahl ist, liegt bei $(1/4)$<sup>k</sup>. 
>Durch jede Iteration wird $k$ erhöht und dadurch die Wahrscheinlichkeit, dass $n$ eine Primzahl ist, höher.

#crypto #DMII #primzahltest #fermat #primzahl