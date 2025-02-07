# <font color = "orange">AufS - 13.01.2025</font>

Man kann die Zustände eines Automaten in einer Tabelle darstellen.

![[AuFS - 03 - Deterministische Endliche Automaten.pdf#page=7]]

Alle Start- und Endzustände sollten in S vorkommen, dh $s_0 \in S,F \subseteq S$

$\delta$ ist die Zustandsüberführungsfunktion. 

Die akzeptierte Sprache eines DEA heißt $A_1$ und wird wie folgt ausgedrückt:
$$
L_1=\{a_1a_2a_3a_4a_5,a_1a_2a_3a_4a_6\}
$$
---

Man kann nun auch eine reflexiv-transitive Hülle $R^+$ von $\delta$ bilden. Dies wäre dann $\delta^*$.

Die Berechnung eines Automaten ist abbildbar über die Konfiguration eines Automaten.
$k$ ist die Konfiguration eines Automaten. Ausgegeben wird $S\times\Sigma^*$.

Die *Vorgänger-Nachfolger-Beziehung* $\vdash$ zwischen dem Paar $k$ und $k'$ lässt sich über eine Relation beschreiben:
$$
\vdash\subseteq(S\times\Sigma^*)\times(S\times\Sigma^*)
$$
Dies lässt sich ganz allgemein ableiten zu: 
$$
k\vdash k' = (s,w)\vdash (s',w')
$$
Die *reflexiv-transitive Hülle* $\vdash^*$ für die Relation $\vdash$ ist rekursiv definiert. Für Erklärung siehe [[AuFS - 03 - Deterministische Endliche Automaten.pdf#page=15]]. 
>[!INFO] Anmerkung des Autors
>Hab davon gerade nichts gecheckt, aber das wird schon noch. (Trust)


Wenn die Elemente $w\in L \subseteq\Sigma^*$ vom Startzustand $s_0$ zu einem Endzustand $s_i\in F$ ist die Sprache $L$ als durch den Automaten $A$ akzeptiert.


## Aufgabenbearbeitung #1
a) Welche Sprache erkennt der rechts stehende Automat


>[!INFO] Anmerkung des Autors
>Was zum Fick ist ein Kleene-Stern?? 
>-> Raussuchen und in [[Reguläre Ausdrücke#Die Menge der Regulären Sprachen]] einfügen. Vielleicht [[Kleene-Abschluss#^031945]]??


## <font color = "lightblue">Nacharbeitung - Aufgaben</font>
- [ ] Kleene-Stern recherchieren
	- Lösung: Es ist tatsächlich $\Sigma^*$ aus [[Kleene-Abschluss#^031945]]
- [ ] Komplementbildung recherchieren
- [ ] Spiegelung recherchieren
- [ ] 