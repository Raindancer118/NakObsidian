# <font color = "orange">AuS - 23.01.2025</font>
Häufungspunkt d . <=> In jeder $\varepsilon$-Umgebung von a liegen unendlich viele Folgen-Glieder.
Thema Folgen abgeschlossen!

---
## Reihen
Die unendliche Summe ist ein Quadrat, das immer weiter in vier weitere Quadrate aufgeteilt wird.

## Das Summenzeichen
Die Summe von 1 bis 19 soll dargestellt werden in einem Summenzeichen. So wird geschrieben:
$$
\sum_{k=2}^{11}(2k-3)
$$

Wenn man das Summenzeichen auf einer Summe hat, dann lässt sich dieses aufspalten in zwei identische Summenzeichen mit je einem der beiden Summanden. Dasselbe gilt für eine Subtraktion.

Das Symbol für eine unendliche Reihe ist $$\sum_{n=1}^{\infty}a_n$$. $a_n$ ist dabei ein Glied der Reihe und $s_n$ heißt Teilsumme oder auch Partialsumme der Reihe.

Eine Reihe ist **[[Konvergenz|konvergent]]**, wenn ihre Teilsummenfolgen **[[Konvergenz|konvergent]]** sind.

Eine Reihe ist dann **divergent**, wenn sie nicht **[[Konvergenz|konvergent]]** ist. 
Die Folien dazu sind [[Folien.pdf#page=38]].

### Arithmetische Reihe
Eine arithmetische Reihe beruht auf einer arithmetischen Folge.
### Geometrische Reihe
Formel für die Teilsummenformel:
$$
\frac{q^{n+1}-1}{q-1}
$$

Für eine geometrische Reihe $$a_0 \sum_{n=0}^\infty q^n$$
ergibt sich als Teilsumme $$s_n=a_0*\frac{q^{n+1}-1}{q-1}$$. Frage: Wann ist die Teilsummenfolge **[[Konvergenz|konvergent]]**?$$\lim\limits_{n \to \infty} s_n = \lim\limits_{n \to \infty} a_0 * \frac{q^{n+1}-1}{q-1}=a_0*\lim\limits_{n \to \infty}\frac{q^{n+1}-1}{q-1}$$. Für $|q| < 1$ gilt $\lim\limits_{n\to\infty}q^{n+1}=0$. Daraus ergibt sich ![[PXL_20250123_161300181.MP~2.jpg]]. Damit lässt sich nun endlich errechnen, dass unser Quadrat von vorher gegen 2 **[[Konvergenz|konvergiert]]**.

### Finanzmathematik - 1
Geld hat einen Zeitwert. Wenn ich Geld schon heute haben, kann ich es direkt nutzen und es beispielsweise anlegen.

In der Finanzmathematik sollen wir das Ergebnis immer auf zwei Dezimalstellen runden.

Zinssatz $i$ - Nominalzins
Zinsrate $r = 1 +i$
Anzahl Jahre $n$
Anzahl Zinsperioden/Jahre $m$ 

Aufgabe: Verkauf einer Maschine: Welches Angebot ist das günstigste?
Angebot A: Sofort 35.000 EUR und 15.000 EUR in 3 Jahren
Angebot B: In einem Jahr 45.000 EUR und in 2 Jahren 5.000 EUR
Vergleichszinssatz $3\%$

A -
**Heute**
35.000 EUR
**In einem Jahr** 
36.050 EUR
**In zwei Jahren**
37.131,50 EUR
**In drei Jahren**
53.245,45 EUR

B-
**Heute**
0 EUR
**In einem Jahr** 
45.000 EUR
**In zwei Jahren**
51.350 EUR
**In drei Jahren**
52.890,50 EUR