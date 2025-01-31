# <font color = "orange">AuD - 31.01.2025</font>
```
for (int i = 0;i < n-1;i++) { 
	for (int j = 0;j < n;j++) {
		if (A[j]<A[i]) {
			count[i]++
		}else{
			count[j]++
		}
	}
	S[count[i]] = A[i]
}
```
>[!WARNING] Sowas hier sollte problemlos möglich sein.
## Komplexitätsanalyse
1. $n$ ermitteln. $n$ ist dabei die Anzahl der Elemente
2. Basisoperation ermitteln
3. Best-Worst-Average-Case ermitteln
	1. Best = Worst = Average
4. Häufigkeit der Ausführung der Basisoperation herausfinden
	1. $$T(n):\sum_{i=0}^{n-2}\sum_{j=i+1}^{n-1}1=\sum_{i=0}^{n-2}n-i-1$$
	$$=1+\dots n-1 = \sum_{i=0}^{n-1}=\frac{(n-1)*n}{2}\approx\Theta(n^2)$$

$\Theta$ - Best=Worst=Average
$\Omega$ - Kann nicht besser werden
$O$ - Kann nicht schlimmer werden

>[!QUOTE] "Da ich das an dieser Stelle nicht an die Tafel schreiben möchte, nutze ich die Programmierumgebung für BWLer - Excel."

## Hashing
```
Map<String,Person> Verzeichnis = new HashMap<>();
Verzeichnis.put("A57321",hugo);
Verzeichnis.get ´("A57321")
```

>[!HINT] Der Key
Der Key einer HashMap muss ein `hashcode()` sein und `equals(...)`. Die `equals(...)`-Methode muss dabei implementiert und überschrieben werden, die die Identifizierung von Objekten regelt.

Hashing wird in Dictionaries sehr viel verwendet mit den Operationen `find`, `insert` oder `delete`. In Hashs können Daten in konstanter Laufzeit gefunden werden.

In einer Hashtabelle werden Schlüssel von Daten auf eine vergleichsweise kleine Tabelle übertragen.

Eine Hashfunktion sollte möglichst leicht und schnell zu berechnen sein und die Hashwerte sollten möglichst gleichmäßig verteilt werden.

Gute Hashfunktionen erzeugen möglichst wenige Kollisionen, ganz grundsätzlich sind diese allerdings nicht vermeidbar.

Der *Load Factor* $\alpha = n/m$ besagt die durchschnittliche Listenlänge.
Der Load Factor sollte in der Nähe von 1 gehalten werden.
>[!QUOTE] Wie viele Plätze von wie vielen sind belegt?

>[!WARNING] Der MD5-Hash gilt als unsicher, da jemand alle Hashes von MD5 durchgerechnet hat.
### Open Hashing
In eine Speicherzelle können mehrere Elemente geschrieben werden. 
**Effizienz von Open Hashing**
### Closed Hashing
Nur ein Schlüssel pro Zelle möglich und bei einer Kollision wird eine andere Zelle gesucht. 
#### Linear Probing / Lineares Sondieren:
Finde nächste freie Zelle.
Durchsuchen ist nun sehr Performance-Intensiv
#### Quadratic probing / Quadratisches Sondieren
Suche nach freien Zellen in quadratisch wachsenden Abständen
#### Double Hashing
Schlüssel wird mehrfach durch Hashes gejagt.

## Bearbeitung Aufgabe
Aufgrund weniger Hash-Positionen kommt ein Load Faktor von ca 16.000 zustande.