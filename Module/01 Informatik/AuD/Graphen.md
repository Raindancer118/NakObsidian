#tbcompleted 
# <font color = "orange">Graphen</font>
>[!INFO] Definition
>Graphen ist eine Datenstruktur, die verwendet wird um Beziehungen zwischen Objekten darzustellen.
## Bestandteile
Ein Graph besteht aus:
- Punkten Z.b. (a,b,c,d,e,f), auch genannt:
	- Ecken
	- Knoten
- Verbindungen, auch genannt:
	- Kanten
![[Pasted image 20250118180908.png]]
## Eigenschaften
>[!INFO] Definition
>Eigenschaften die Graphen zugeordnet werden um sie zu kategorisieren.  
### Ungerichtet
>[!INFO] Definition
>Es gibt keine Pfeile an den Verbindungen.

>[!example]
>B ist [[Adjazenz|Adjazent]] zu A und A zu B.
>![[Pasted image 20250118180908.png]]

### Gerichtet
>[!INFO] Definition
>Die Verbindungen/kanten sind Pfeile.
>Die Verbindungen können einwegig sein. 
>[[Adjazenz]] kann betrachtet werden wie ein weg.

>[!example]
>B ist [[Adjazenz|Adjazent]] zu A , aber A nicht zu B.
>![[Pasted image 20250118180752.png]]

### Schleife
>[!INFO] Definition
>Ein Knoten ist mit sich selber verbunden.

### Mehrfachkanten
>[!INFO] Definition
>Mehrere Verbindungen zwischen denselben Knoten

>[!example]
>![[Pasted image 20250118182655.png]]
### Gewichtung
>[!INFO] Definition
>Den Verbindungen wird einen Zahlenwert (Gewicht, Kosten, Entfernung) zugeordnet.
>

>[!example]
>![[Pasted image 20250118182001.png]]


### Zusammenhängend
>[!INFO] Definition
>Alle Knoten sind verbunden.

#### Stark Zusammenhängend
>[!INFO] Definition
>Alle Knoten sind ereichbar 
#### Schwach Zusammenhängend
>[!INFO] Definition
>Alle Knoten sind verbunden aber nicht unbedingt ereichbar.

### Einfacher Pfad 
>[!INFO] Definition
>Es gibt keine Verbindungswiederholung.
>Jeder Knoten wird höchstens einmal besucht.