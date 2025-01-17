# <font color = "orange">Sortierverfahren</font>
>[!INFO] Definition
>Es gibt verschiedene Sortierverfahren, die für Daten oder auch Dinge verwendet werden können. 

>[!INFO] Eigenschaften von Sortierverfahren
>- Stabil (Wenn zwei Elemente gleich sind, dann erhalten sie die gleiche Reihenfolge)

>[!TIP] **Merge Sort** und **Quick Sort** sind die schnellsten Sortierverfahren der Welt.
## Merge Sort
>[!INFO] Grundlegende Idee
>Das Array in zwei Hälften Teilen und in zwei weitere Arrays teilen. Anschließend werden diese beiden Arrays wieder geteilt und so lange, bis alle Arrays jeweils nur noch ein Element beinhalten.
>Anschließend werden diese Arrays wieder zusammengefügt, in einer neuen Reihenfolge.

>[!STRENGTHS]
>- Implementierung *ohne Rekursion* möglich
>- Stabiles Sortierverfahren 
>- Arrays werden *sequentiell* verarbeitet

>[!FORMULA] Pseudocode
>```
>//Sorts array A[0..n - 1] by recursive mergesort
>//Input: An array A[0..n - 1] of orderable elements
>//Output: Array A[0..n - 1] sorted in nondecreasing order
>if n > 1
>	copy A[0..[n/2] - 1] to B[0..[n/2] - 1]
>	copy A[[n/2]..n - 1] to C[0.. [n/2] - 1]
>	Mergesort(B[0..[n/2] - 1])
>	Mergesort(C[0..[n/2] - 1])
>	Mergesort(B,C,A)
>```

>[!HINT] Die Sortierreihenfolge ist am Ende eigentlich auch egal; die kann von außen mitgegeben werden, sodass der Algorithmus vielseitig einsetzbar ist.

>[!WARNING] Der Speicherplatz von Mergesort liegt bei log(n).

Für mehr Informationen zu Merge Sort gern auf den Folien [[AuD05_WINF.pdf#page=6|hier]], und auf den weiterführenden Folien nachsehen.
## Quick Sort
## Selection Sort
## Insertion Sort
>[!QUOTE] Ich nehme ein Element und füge es in ein sortiertes Array ein.
