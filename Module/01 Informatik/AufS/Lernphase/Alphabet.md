# <font color = "orange">Alphabet</font>
Ein Alphabet ist eine Menge von Zeichen, aus denen Zeichenreihen gebildet werden können. 
Die Zeichen aus den Alphabeten können als Eingabe oder Ausgabe von endlichen Automaten genutzt werden.

Ein Alphabet, bezeichnet mit dem Zeichen $\sum$, beschreibt eine **abgeschlossene** und **endliche** Menge von Zeichen.

>[!HINT] Abgeschlossenheit
>Abgeschlossenheit heißt, dass das Ergebnis von Mengenoperationen die Menge nicht verlässt, egal, welche Operation angewendet wird.
## Darstellung
#### Extensional
Ein Alphabet kann **extensional** dargestellt werden, indem einfach alle seine Elemente aufgelistet werden in der üblichen Mengenschreibweise:
$$\sum=\{0,1,2,3,4,5,6,7,8\}$$
#### Intensional
Eine **intensionale** Darstellung liegt vor, wenn eine Teilmengenbeziehung mit einer "filternden" oder auch eingrenzenden Eigenschaft genutzt werden kann, um die Menge exakt zu beschreiben. Dies nennt sich auch "**Aussonderung**"

>[!DANGER] Achtung
>Das **leere Wort $\varepsilon$** ist immer in einem Alphabet enthalten!
## Kleenesche Hülle
Die Kleenesche Hülle eines Alphabetes ist das Alphabet, plus alle Worte, die sich aus der Konkatenation von beliebigen Zeichen aus diesem Alphabet bilden lassen, inklusive dem leeren Wort.