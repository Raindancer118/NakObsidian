```
//Sorts array A[0..n - 1] by recursive mergesort
//Input: An array A[0..n - 1] of orderable elements
//Output: Array A[0..n - 1] sorted in nondecreasing order
if n > 1
	copy A[0..[n/2] - 1] to B[0..[n/2] - 1]
	copy A[[n/2]..n - 1] to C[0.. [n/2] - 1]
	Mergesort(B[0..[n/2] - 1])
	Mergesort(C[0..[n/2] - 1])
	Merge(B,C,A)
```
^ Originaler Mergesort-Algorithmus

````
//Sorts array A[0..n - 1] by recursive mergesort
//Input: An array A[0..n - 1] of orderable elements
//Output: Array A[0..n - 1] sorted in decreasing order
if n > 1
	copy A[0..[n/2] - 1] to B[0..[n/2] - 1]
	copy A[[n/2]..n - 1] to C[0.. [n/2] - 1]
	Mergesort(B[0..[n/2] - 1])
	Mergesort(C[0..[n/2] - 1])
	Merge(B,C,A)
	return A.getFirst()
```
^ Neuer Mergesort-Algorithmus mit Return-Ausgabe