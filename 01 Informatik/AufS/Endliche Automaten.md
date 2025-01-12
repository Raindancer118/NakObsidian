# <font color = "orange">Endliche Automaten</font>
Endliche Automaten sind im Endeffekt endliche Graphen. 
Sie haben verschiedene Zustände. Wir wollen vom Start des Automaten zu dessen doppelt umkreisten Ziel.
Es lassen sich verschiedene Zustände anzeigen und man kann endliche Automaten beweisen.

Am Ende sollte jede Möglichkeit im Automaten aufgeschrieben sein.
Hier ein Beispiel für einen endlichen Automaten:
![[AuFS - 01 - Einführung.pdf#page=19]]

Dabei wird jeder Zustand nur einmal aufgelistet.

Endlich heißt dabei, dass jede Möglichkeit hingeschrieben werden kann.

>[!EXAMPLE] Lichtschalter
>Lichtschalter sind endliche Automaten mit dem einen Zeichen "Drücken" im Alphabet.

# Deterministische Endliche Zustandsautomaten
Diese sind ein *Quintupel* bestehend aus: 
$$
(\sum,S,\delta,s_0,F)
$$
$\sum$ bezeichnet dabei das [[Alphabete|Eingabealphabet]].
$S$ ist die [[Zustandsmenge]]
$\delta : S*\sum -> S$ ist die [[Zustandsüberführungsfunktion]].
$S_0$ ist der Startzustand.
$F$ ist ein Endzustand.

# Generelle Informationen
Es gibt endliche Automaten, die einen Speicher haben.