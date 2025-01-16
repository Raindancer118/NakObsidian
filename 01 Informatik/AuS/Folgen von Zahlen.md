# <font color = "orange">Folgen von Zahlen</font>
>[!INFO] Definition "Folge"
>Eine Folge ist eine Funktion einer [[DM II - Abbildung|Abbildung]] von $\mathbb{N}$ in $\mathbb{R}$.
>
>Folgen sind Funktionen.

## Schreibweise
Aufzählend: $(\frac{1}{2},\frac{1}{2^2},\frac{1}{2^3},\dots)$         $a_n:=\frac{1}{2^n}$
Nicht aufzählend: $(a_n)_{n\in\mathbb{N}}$

## Folgenglieder
Die Reellen Zahlen $a_n:=f(n)$ heißen Glieder der Folge.
Die Menge, die ausschließlich die Folgenglieder enthält, heißt *Menge der Folgenglieder* einer Folge f, dies wäre also: $\{a_{i_1},a_{i_2},a_{i_3}\}$
>[!WARNING] Eigentlich richtig wäre hier "Menge der Folgengliederwerte".

Es ist auch zugelassen, dass der Index einer Folge auch mit $0$ oder $n>1$ beginnen kann. 

>[!WARNING] Folgen sind mit einer Bildungsvorschrift versehen, die angibt, wie diese Folge zu bilden ist.
## Darstellung von Folgen
Folgen können anhand eines Graphen dargestellt werden. Dies kann ein- oder zweidimensional passieren. Geogebra kann da verwendet werden.

Folgen von Zahlen können in aufzählender und nicht aufzählender Schreibweise geschrieben werden.

## Beispiele von Folgen
>[!EXAMPLE] Aktienkurse
>Aktienkurse sind eigentlich eine Folge von Werten, keine kontinuierliche Kurve.

>[!EXAMPLE] Rekursion
>Eine Rekursion ist eine Folge von Werten ab einem bestimmten Wert. Diese Folge kommt dadurch zustande, dass der jeweils nächste Wert mithilfe des jeweils letzten berechnet wird.
>
>**Example**
>$a_{n+1}=\frac{1}{2}(a_n+\frac{2}{a_n})$
>$a_1=1$
>$a_2=\frac{3}{2}$
>$\dots$
>*Welche Tendenz ergibt sich? -> 1 oder -> 2?*
>*Annahme: Die Folge der $a_n$ nähren sich immer mehr einer (unbekannten) Zahl $a$.*

>[!FORMULA] Fibonacci-Zahlen
>Die Fibonacci-Zahlen sind eine besondere Folge von Zahlen, die sich anhand der folgenden Formel errechnen lassen:
>$f_0=0$
>$f_1=1$
>$f_n=f_{n-1}+f_{n-2}$ n ist dabei größer gleich 2

## Rechnen mit Folgen
>[!HINT] Es wird elementeweise gerechnet. 

Summe: $f_1 + f_2 = (a_n) + (b_n) := (a_n + b_n) = (\frac{1}{n} + \frac{n^2 + 1}{n}) = (\frac{n^2 + 2}{n})$
Produkt: $f_1 * f_2 = (a_n)*(b_n):=(a_n * b_n) = (\frac{1}{n} * \frac{n^2 + 1}{n}) = (\frac{n^2 + 1}{n^2})$
## Monotonie
Wenn $a_n \leq a_{n+1}$, ist eine Folge *monoton wachsend*.
Wenn $a_n < a_{n+1}$, ist eine Folge *streng monoton wachsend*.
Im Umkehrschluss kann es selbstverständlich auch *monoton fallende* und *streng monoton fallende* Folgen geben. Weiterhin kann es selbstverständlich auch *monotone* Folgen (monoton wachsend oder monoton fallend) geben oder auch *streng monotone* Folgen (streng monoton wachsend oder fallend.)
Monoton wachsend und Monoton fallend: *konstante* Folge.
## Schranken
Es kann sein, dass eine Folge $f$ durch reelle Zahlen $s$ und $S$ mit $S$ als *oberer Schranke* und $s$ als *unterer Schranke* **beschränkt** heißt. Dies gilt allerdings **nur für reelle Folgen**.
$$
s\leq a_n \leq S
$$
Dabei gilt:
$$
\forall_n \in \mathbb{N}
$$
>[!WARNING] Eine Folge gilt nur dann als beschränkt, wenn $f$ **sowohl durch eine untere als auch eine Obere Schranke** begrenzt ist.

## Eigenschaften reeller Folgen
(Siehe Folien [[Folien.pdf#page=22|hier]])
Wenn wir eine riesige $\varepsilon$-Umgebung schaffen, dann sind natürlich alle Folgenglieder in der Folge. Ist dies allerdings nicht der Fall, dann haben wir eine *Zweiteilung* der Folge in ein *Anfangsstück* und ein *Endstück*.

Das *Anfangsstück* der Folge ist endlich und das *Endstück* ist unendlich.
>[!QUOTE] Die Endlichkeit bleibt draußen und wir beherrschen die Unendlichkeit.

Folgen mit der Eigenschaft, dass für jede beliebig kleine oder große $\huge\varepsilon$-Umgebung einer Zahl a (Beispiel: 0) die Folge in ein endliches Anfangsstück und ein unendliches Endstück geteilt wird, werden wir als *[[konvergent]]* bezeichnen.