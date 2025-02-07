# <font color = "orange">AuD - 07.02.2025</font>
- Coin-Row-Problem $\neq$  Wechselgeldproblem

| 0   | 1   | 2   | 3   | 4   | 5   |
| --- | --- | --- | --- | --- | --- |
| -   | 5   | 1   | 2   | 10  | 6   |
| 0   | 5   | 5   | 7   | 15  | 15  |
>[!QUOTE] "Eigentlich immer da, wo man eine Zahl doppelt sieht, immer die nehmen."

### Schachbrettproblem
Laufzeitkomplexität: $\Theta(n^2)$ und Speicherplatzkomplexität: $n^{\Theta(n^2)}$.
Formel: $F(x,y) = F(x-1,y)+F(x,y-1)$.

### Rucksackproblem
Es gibt eine Anzahl von Objekten, jedes Objekt ist einmalig und von jedem Objekt ist der Preis bekannt. Die wertvollste Menge soll mitgenommen werden. Dabei gibt es nur ganzzahlige Gewichte.
Der Rucksack ist allerdings genormt und kann nur eine bestimmte Menge halten.

Welche Gegenstände wurden eingepackt

|                | Kapazität | 0   | 1    | 2    | 3    | 4    | 5    |
| -------------- | --------- | --- | ---- | ---- | ---- | ---- | ---- |
|                | 0         | *0* | *0*  | *0*  | *0*  | *0*  | *0*  |
| Gegenstand 1   | 1         | *0* | *0*  | *12* | *12* | *12* | *12* |
| Gegenstand 1-2 | 2         | *0* | *10* | *12* | *22* | *22* | *22* |
| Gegenstand 1-3 | 3         | *0* | *10* | *12* | *22* | *30* | *32* |
| Gegenstand 1-4 | 4         | *0* | *10* | *15* | *25* | *30* | *37* |


