# <font color = "orange">Klausur 2020 Neuhaus</font>
1)
a) 
G ist stark zusammenhängend, da sich von jedem Knoten jeder andere Knoten über einen gerichteten Pfeil erreichen lässt.

b)

| Kante | Könnte entfernt werden (j/n) |
| ----- | ---------------------------- |
| (d,d) | j                            |
| (c,b) | j                            |
| (a,c) | j                            |
| (a,d) | j                            |
c) 
1. Ungewichtet
2. Nicht Zyklenfrei
3. / 
4. / 

d)

| Zyklenlänge | Beispiel                                              |
| ----------- | ----------------------------------------------------- |
| 1           | (d,d)                                                 |
| 2           | /                                                     |
| 3           | (c,b),(b,a),(a,c)                                     |
| 4           | /                                                     |
| 5           | (a,d),(d,f),(f,e),(e,b),(b,a)                         |
| 6           | (a,c),(c,d),(d,f),(f,e),(e,b),(b,a)                   |
| 7           | /                                                     |
| 8           | (a,c),(c,d),(d,f),(f,e),(e,b),(b,a),(a,c),(c,b),(b,a) |

2)
```
public boolean beideKanten(int[][] A) {
	int doubleCounter = 0;
	int n = A.length;
	for (int x = 0; x < n;x++) {
		for (int y = 0; y < n; y++) {
			if (x == y) break;
			if (A[x][y] == 1) {
				if (A[y][x]) doubleCounter++;
			
			}
		}
	}
	if(doubleCounter > n) return true;
	return false;
}
```

falsch; keine Punkte

3)
a) 
Die Laufzeitkomplixität von von f beträgt 























































| Länge | Beispiel                                   |
| ----- | ------------------------------------------ |
| 1     | (B,B)                                      |
| 3     | (E,F),(F,C),(C,E)                          |
| 4     | (b,a),(a,d),(d,e),(e,b)                    |
| 6     | (b,a),(a,d),(d,e),(e,f),(f,c), (c,b)       |
| 7     | (b,a),(a,d),(d,e),(e,f),(f,c), (c,e),(e,b) |

c)
(b,b),(c,e),(e,b)

$i<m$
$$
\huge\sum^{m-1}_{i=0} \sum^{n}_{j=1} \sum^{\sqrt{n}}_{k=1}1 = \sum^{m-1}_{i=0} \sum^{n}_{j=1}\sqrt{n} = \sum^{m-1}_{i=0}n\sqrt{n} = \sqrt{n}mn
$$

Algorithmus, der immer gleich läuft, unabhängig von der Eingabe, dann $\Theta$. Sonst Groß O für Worst Case und $\Omega$ für Best Case.

$42n=2nlog_2n +4n$ |$-4n$
$38n = 2nlog_2n$ |:2n
$19 = log_2n$ 
$2^{19} = n$
