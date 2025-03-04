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
public static boolean mehrAlsDieHälfteDoppelt (int[][] A) {
	int n = A.length;
	int aC = 0; //aC for ArrayCounter
	int dC = 0; //dC for Doppel-Counter
	for (int i = 0; i < n; i++) {
		if(aC != i) {
			if((A[aC][i] == 1) && (A[i][aC] == 1)) {
				dC++;
			}
		}
		aC++;
	}
	return (dC > n/2);
}
```

falsch; keine Punkte

3)
a) 
Die Laufzeitkomplixität von von f beträgt 