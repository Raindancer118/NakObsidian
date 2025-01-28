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

^167bf7

>[!FORMULA] Irreflexiv
>Eine Relation ist *irreflexiv*, wenn die Schnittmenge zwischen $Id_M$ und $R$ *leer* ist. Das heißt, es darf **keine identischen Paare in $R$ geben**.  Man sagt auch, dass eine Relation *irreflexiv* ist, wenn $Id_M \not\subseteq R$.

>[!FORMULA] Symmetrisch
>Eine Relation heißt *symmetrisch*, wenn *$R$ invers* **Teilmenge** von R ist. Das heißt, wenn zu jedem Paar auch das inverse Paar in der Relation ist. Man schreibt auch $R^-1 \subseteq R$.
>In einer Matrixdarstellung würde eine symmetrische Relation an der Mitteldiagonale gespiegelt.

^bf34f9

>[!FORMULA] Asymmetrisch
>Eine Relation heißt *asymmetrisch*, wenn *$R$ invers* **nicht** in $R$ liegt. Das heißt, wenn das inverse Paar zum aktuellen Paar eben nicht in der Relation liegt. Man schreibt auch $R \cap R^-1 = \emptyset$.

>[!DANGER] ~~Symmetrisch~~ $\to$ Asymmetrisch

>[!FORMULA] Antisymmetrisch
>Eine Relation heißt *antisymmetrisch*, wenn die Schnittmenge zwischen $R$ und $R$ invers $Id_M$ bildet. Man schreibt dabei $R \cap R^-1 \subseteq Id_M$. 

>[!FORMULA] Transitiv
>Eine Relation heißt *transitiv*, wenn $R \circ R \subseteq R$. Das heißt, wenn $R$ verkettet mit sich selbst wieder in $R$ ist, ist dies eine *transitive* Relation. Im Pfeildiagramm impliziert eine Transitivität von zwei Relationen eine Verbindung zwischen all ihren Elementen. 
>>[!EXAMPLE]
>>Es gibt die zwei Relationen $(a,b)$ und $(b,c)$. Nun lässt sich aufgrund der Transitivität sagen, dass auch eine Relation $(a,c)$ existieren muss.

^b056e9

