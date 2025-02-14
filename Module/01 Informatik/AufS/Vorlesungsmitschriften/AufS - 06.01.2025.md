# <font color = "orange">AufS - 06.01.2025</font>
- zweite Vorlesung am Freitag
- Insgesamt 9 Veranstaltungen
- Abschluss mit Klausur am Anfang zu Q2
- Was nicht erzählt wird, wird nicht abgeprüft
- Wenn was erzählt wird, **was nicht auf den Folien steht, ist das trotzdem prüfungsrelevant**
- Als Hauptmaterial wird genutzt [[Grundkurs Theoretische Informatik.pdf]]
- Ca **50% Durchfallquote** mit einer eher schlechten Durchschnittsnote.
- Grundelemente:
	- [[Alphabete]]
	- [[Wörter]]
	- [[Sprachen]]
- [[Endliche Automaten]]
- [[Kellerautomaten]]
- [[Turing-Maschinen]]
- [[Reguläre Ausdrücke]]
	- [[Reguläre Ausdrücke#Notation]]
	- [[Reguläre Ausdrücke#Rechenregeln]]
	- [[Reguläre Ausdrücke#Äquivalenz von Automaten und Ausdrücken]]
- [[Grammatiken]]

- Wir lernen die theoretischen Elemente, weil wir die Theorie verstehen und uns bereits im Voraus schon ausdenken, bevor wir sie dann in einem Code niederschreiben können sollen.

## Church-Turing-These
Turing Berechenbarkeit -> Das, was ein Computer erreichen kann.
>[!Hint] Turing Berechenbarkeit
>Berechenbar für einen Computer ist jede Funktion, die wir uns einfach niederschreiben können.


>[!QUOTE] "Testen ist besseres Raten"

Wir sollten beweisen können, dass unser Programm funktioniert, sodass wir nicht testen müssen.

>[!QUOTE] "Halt ist keine berechenbare Funktion."

^c2f512

>[!IMPORTANT] [[Halteproblem]] ganz stark #klausurrelevant

Wie **teuer** ist mein Programm? 
- Teuer berechnet man anhand von zwei Faktoren: Zeit, Rechenkraft

Fragen, die man sich in der Komplexitätsbetrachtung stellt: Wie viel Speicher braucht denn mein Problem eigentlich?

Matrixmultiplikation ist **nicht** klausurrelevant.

Es könnte rein theoretisch ein Programm geben, das nur $n^2$ Schritte benötigt, doch eine Berechnung mit $n^3$ Schritten ist vollkommen indiskutabel unmöglich.
-> [[AuFS - 01 - Einführung.pdf#page=13]]

## Endliche Automaten
Aufschrieb zu endlichen Automaten direkt in [[Endliche Automaten]].
Wir haben einen ersten endlichen Automaten erstellt, der die Aufgabe hat, eine Eintrittskarte fürs Schwimmbad dann auszugeben, wenn mehr als 2€ eingeworfen wurden.

In endlichen Automaten sollen korrekte Sätze erkannt werden.

Endliche Automaten akzeptieren Worte, die nach ihrer vollständigen Abarbeitung in einem Endzustand auskommen. Gleichzeitig lässt sich die Sprache $L$ des Automaten beschreiben als die Menge aller von ihm akzeptierten Wörter,

Eine **Konfiguration** $k$ beschreibt den aktuellen Stand der Verarbeitung. Dies wird wie folgt aufgeschrieben:
$K_0 = (S_0,50,50,100)$
$K_1=(S_50,50,100)$
...
$(S_200+,-)$

Wir reden zunächst über Automaten und anschließend über Grammatik. Das sollte man nicht durcheinander bekommen, aber das passiert leider trotzdem vielen.

## Entscheidungsprobleme
Probleme, die auftreten können, die aber durch einen endlichen Automaten immer über Algorithmen lösbar sind:
- Wortproblem
- Leerheitsproblem
- Leerheitsproblem
- Endlichkeitsproblem
- Äquivalenzproblem

Die Sprache eines endlichen Automaten kann unendlich sein.

## Tools
In der Vorlesung könnte https://www.jflap.org/ eine Hilfe sein.