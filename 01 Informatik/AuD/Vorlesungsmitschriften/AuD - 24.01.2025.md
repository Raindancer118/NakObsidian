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