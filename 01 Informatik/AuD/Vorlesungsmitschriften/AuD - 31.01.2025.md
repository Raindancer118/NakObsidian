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