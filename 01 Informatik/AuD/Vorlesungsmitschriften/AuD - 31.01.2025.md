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
2. 