# <font color = "orange">AuD - 24.01.2025</font>
Bearbeitung der geringsten Distanz zwischen zwei Elementen:
```
Function minDistance(A[0 ... n-1])
	min = int.maxValue
	for (int i;i < n-1;i++) {
		for (int j = i+1;j < n;j++){
		if (distance(A[i],A[j])<min) {
			min = distance(A[i],A[j])
			}
		}
	}
```

Die Gleichheit zwischen zwei Elementen ist eine gewisse Art Relation.

## Median Bestimmung
### Bruteforce
```
Function median(A[0 ... n-1]) {
	K = |n/2|
	for (int i=0;i < n; i++) {
		numssmaller=0;
		numsequal=0;
		for (int j=0;j < n; j++) {
			if (A[j] < A[i]){
				numssmaller++;
			} else if (A[j] == A[i]) {
				numsequal++
			}
		}
	}
	if(numssmaller = K) {
		return A[i];
	}
}
```
### Vorsortiert
Einfach den mittleren Wert herausholen: A[n/2]

## Min / Max
### Bruteforce
Alle anschauen und min und Max bis zum Ende merken.
$\Theta(n)$
### Divide & Conquer
```
Min(A[0...n-1]) = minimum(Min(A[0 ... [(n-1)/2]]),Min(A[[(n-1)/2]+1...n-2]))
```
Ausführungshäufigkeit der Basisoperation:
```
T(n) = 1 + 2 * T(n/2)
T(1) = 0
T(2^K) = 1 + 2 * T(2^{K-1})
= 1 + 2 (1 + 2T (2^{K-2}))
= 1 + 2 + 4T (2^{K-2})
= 1 + 2 + 4 + 8T (2^{K-3})
= 2^3 - 1 + 8T (2^{K-3})
= 2^{K-1} = n - 1
```