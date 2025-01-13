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
$k$ ist die Konfiguration eines Automaten. Ausgegeben wird $S