---
aliases:
  - Relation
  - Relationen
---
# <font color = "orange">Relation</font>
>[!INFO] Definition
>Eine Relation ist das Modell einer Beziehung zwischen zwei Objekten. Sie sind zunehmend nicht nur in der Mathematik, sondern aufgrund von Beziehungen in SQL auch für Informatiker interessant.
>
>Mithilfe von Relationen lassen sich in der Mathematik **[[DM II - Ordnungen|Ordnungen]]** und **[[DM II - Äquivalenz|Äquivalenzen]]** beschreiben. Auch **[[DM II - Abbildung|Abbildungen]]** sind Relationen, wenn auch spezielle.

>[!HINT] Relationen sind in der Basis zweistellige Prädikate.
>Das heißt, dass eine Relation aus zwei Objekten, $x$ und $y$, besteht, die in einer unbekannten und vollkommen abstrakten Beziehung zueinander stehen.
>Also: 
>$$
>(x,y) \in R
>$$
>>[!INFO] Anmerkung des Autors
>>Die Beziehung zwischen $x$ und $y$ muss nicht real anzutreffen sein und ist rein theoretisch. Sie sollte nicht hinterfragt werden.

>[!EXTRA] Merke
>Eine Relation $R$ ist **eine Teilmenge des kartesischen Produktes** aus $M \times N$.
>Das heißt: 
>$$
>R \subseteq M \times N
>$$
>
>$R$ kann dabei allerdings auch eine Teilmenge des kartesischen Produktes aus $M \times M$ sein. Ist dies der Fall, ist **$R$ eine Relation auf $M$**.

## Eigenschaften von Relationen
>[!FORMULA] Reflexiv
>Eine Relation ist *reflexiv*, wenn sie alle identischen Paare beinhaltet. $Id_M$ ist dabei die Menge der identischen Relationen auf $M$. Man sagt auch, wenn $Id_M \subseteq R$. 

>[!FORMULA] Irreflexiv
>Eine Relation ist *irreflexiv*, wenn die Schnittmenge zwischen $Id_M$ und $R$ *leer* ist. Das heißt, es darf **keine identischen Paare in $R$ geben**.  Man sagt auch, dass eine Relation *irreflexiv* ist, wenn $Id_M \not\subseteq R$.

>[!FORMULA] Symmetrisch
>Eine Relation heißt *symmetrisch*, wenn $R$ *invers* Teilmenge von R ist. Das heißt, wenn zu jedem Paar auch das inverse Paar in der Relation ist. Man schreibt auch $R^-1 \subseteq R$.

>[!FORMULA] Asymmetrisch
>Eine Relation heißt *asymmetrisch*, wenn *$R$ invers* **nicht** in $R$ liegt. Das heißt  