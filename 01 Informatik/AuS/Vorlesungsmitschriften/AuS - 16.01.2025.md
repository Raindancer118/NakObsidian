# <font color = "orange">AuS - 16.01.2025</font>
Behauptung: 
$$
\sqrt{b}-\sqrt{a} < \sqrt{b-a}
$$
$$
\Leftrightarrow(\sqrt{b}-\sqrt{a})^2 < b-a
$$
$$\Leftrightarrow(\sqrt{b}-\sqrt{a})(\sqrt{b}-\sqrt{a}) < b-a$$
$$\Leftrightarrow b-2\sqrt{b}\sqrt{a} + a < b - a$$ |-b
$$\Leftrightarrow -2 \sqrt{b}\sqrt{a} < -2a$$
| :2 
$$\Leftrightarrow \sqrt{b}\sqrt{a} > a$$
$$\Leftrightarrow b*a > a^2$$

## Kurzwiederholung:
$$
\mathbb{N}_0\mathbb{,N, Z, Q, R}
$$

$|x|$    -> Betrag -> Fallunterscheidung!

$\varepsilon$-Umgebung einer Zahl $a\in\mathbb{R}: U_3 (a): = \{x | x-a|<\varepsilon\}$
-> symmetrisches offenes Intervall um $a$.

offene Menge: Randpunkte gehören nicht dazu
abgeschlossene Menge: Randpunkte gehören dazu
$\neg$ offene Menge $\neq$ abgeschlossene Menge
		(gemischte Fälle!)
$\emptyset$ ist offen, $\mathbb{R}$ ist offen und abgeschlossen.
$\mathbb{R}$ mit einem ^ darüber heißt "R-Dach" und es entspricht $\mathbb{R}\cup$

[[Folgen von Zahlen]] sind mit einer Bildungsvorschrift versehen.

Wir hatten letztes Mal bereits die geometrische Darstellung von Folgen bearbeitet. Diese findet sich auf den Folien [[Folien.pdf#page=18|hier]].

Eine **Folge kann auch als Abbildung oder Funktion** definiert werden.

## Neue Vorlesungsinhalte
Erst die hinteren Teile der Folgen sind interessant. 
In den Vorlesungen muss $n\in\mathbb{N}$ nicht danebenstehen, aber in der Klausur wird das erwartet. Wenn wir das allerdings darüber schreiben als Anmerkung ist es okay.

### Monotonie
Wenn $a_n \leq a_{n+1}$, ist eine Folge *monoton wachsend*.
Wenn $a_n < a_{n+1}$, ist eine Folge *streng monoton wachsend*.
Im Umkehrschluss kann es selbstverständlich auch *monoton fallende* und *streng monoton fallende* Folgen geben. Weiterhin kann es selbstverständlich auch *monotone* Folgen (monoton wachsend oder monoton fallend) geben oder auch *streng monotone* Folgen (streng monoton wachsend oder fallend.)
Monoton wachsend und Monoton fallend: *konstante* Folge.

### [[Schranken]]
Es kann sein, dass eine Folge $f$ durch reelle Zahlen $s$ und $S$ mit $S$ als *oberer Schranke* und $s$ als *unterer Schranke* **beschränkt** heißt. Dies gilt allerdings **nur für reelle Folgen**.
$$
s\leq a_n \leq S
$$
Dabei gilt:
$$
\forall_n \in \mathbb{N}
$$
>[!WARNING] Eine Folge gilt nur dann als beschränkt, wenn $f$ **sowohl durch eine untere als auch eine Obere Schranke** begrenzt ist.

### Eigenschaften reeller Folgen
(Siehe Folien [[Folien.pdf#page=22|hier]])
Wenn wir eine riesige $\varepsilon$-Umgebung schaffen, dann sind natürlich alle Folgenglieder in der Folge. Ist dies allerdings nicht der Fall, dann haben wir eine *Zweiteilung* der Folge in ein *Anfangsstück* und ein *Endstück*.

Das *Anfangsstück* der Folge ist endlich und das *Endstück* ist unendlich.
>[!QUOTE] Die Endlichkeit bleibt draußen und wir beherrschen die Unendlichkeit.

Folgen mit der Eigenschaft, dass für jede beliebig kleine oder große $\huge\varepsilon$-Umgebung einer Zahl a (Beispiel: 0) die Folge in ein endliches Anfangsstück und ein unendliches Endstück geteilt wird, werden wir als *[[konvergent]]* bezeichnen.

$$
\forall \varepsilon > 0: \exists n_0 \in \mathbb{N}: \forall n \in \mathbb{N}: n>n_0 \Rightarrow |a_n-a|<\varepsilon
$$
*Konvergenz gegen $a\in\mathbb{R}$*

>[!QUOTE] "Für jede Epsilon-Umgebung, die größer als Null ist, gilt, dass es ein N-Null gibt, das in N ist,"

>[!EXAMPLE]
>$(a_n)n\in\mathbb{N}$
>$a_n:=2+\frac{(-1)^n}{n}$
>$(1,2+\frac{1}{2},2-\frac{1}{3},2+\frac{1}{4},\dots)$
>$\varepsilon = 0,001$

### Rechnen mit Folgen #2
Es gibt einige Rechenregeln für Konvergente Folgen, die sich [[Folien.pdf#page=26|hier]] finden.

>[!INFO] Reziprok
>Reziprok nennt man Quadratzahlen, die als Nenner in einem Bruch stehen.

Wir sollen uns definitiv die Materialien [[Folien.pdf#page=27]] und [[Folien.pdf#page=28]] anschauen und diese auswendig können. 