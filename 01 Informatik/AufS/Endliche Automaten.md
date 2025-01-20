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
## Generelle Informationen
Es gibt endliche Automaten, die einen Speicher haben.

## Typen von Endlichen Automaten
- Akzeptoren
	- DEA
	- NEA
	- $\varepsilon$-EA
- Transduktoren

>[!Danger] Endliche Automaten können nicht bis **$\infty$** zählen. Sie können ausschließlich **endliche** Zustandsmengen abbilden.

>[!TIP] Für jeden DEA gibt es auch ein NEA, der dieselbe Sprache spricht wie der DEA.
## Deterministische Endliche Zustandsautomaten
Diese sind ein *Quintupel* bestehend aus: 
$$
(\sum,S,\delta,s_0,F)
$$
$\sum$ bezeichnet dabei das [[Alphabete|Eingabealphabet]].
$S$ ist die [[Zustandsmenge]]
$\delta : S*\sum -> S$ ist die [[Zustandsüberführungsfunktion]].
$S_0$ ist der Startzustand.
$F$ ist ein Endzustand.

>[!WARNING] DEAs sind im Endeffekt nur spezielle NEAs
## Nicht deterministischer endlicher Zustandsautomat
>[!HINT] Ein NEA ist in der Lage, sich selbst unendlich oft zu klonen.
