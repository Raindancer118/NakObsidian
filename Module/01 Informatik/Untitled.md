# Summenformeln auflösen

## 1. Konstante Summe
**Form:**  
$$
\Large \sum_{i=a}^{b} c
$$  
(Die Summe läuft von \( i = a \) bis \( i = b \), wobei \( c \) eine Konstante ist.)  

**Lösung:**  
$$
\sum_{i=a}^{b} c = c \cdot (b - a + 1)
$$  

**Beispiel:**  
$$
\sum_{i=1}^{n} 3 = 3 \cdot n
$$

---

## 2. Lineare Summe (\( i \)-Summenregel)
**Form:**  
$$
\sum_{i=1}^{n} i
$$  

**Lösung (Gauss-Formel):**  
$$
\sum_{i=1}^{n} i = \frac{n(n+1)}{2}
$$  

**Beispiel für \( n = 5 \):**  
$$
1 + 2 + 3 + 4 + 5 = \frac{5(6)}{2} = 15
$$

---

## 3. Quadratische Summe
**Form:**  
$$
\sum_{i=1}^{n} i^2
$$  

**Lösung:**  
$$
\sum_{i=1}^{n} i^2 = \frac{n(n+1)(2n+1)}{6}
$$  

---

## 4. Geometrische Summe
**Form:**  
$$
\sum_{i=0}^{n} r^i
$$  

**Lösung:**  
$$
\sum_{i=0}^{n} r^i = \frac{r^{n+1} - 1}{r - 1}, \quad r \neq 1
$$  

Falls \( r = 1 \), dann ist die Summe einfach \( n+1 \), weil alle Terme \( 1 \) sind.  

**Beispiel für \( r = 2 \):**  
$$
\sum_{i=0}^{n} 2^i = \frac{2^{n+1} - 1}{2 - 1} = 2^{n+1} - 1
$$

---

## Allgemeine Schritte zum Auflösen von Summen
1. **Vergleiche mit bekannten Formeln** (siehe oben).
2. **Zerlege die Summe**, falls sie mehrere Terme enthält.
3. **Nutze Distributivgesetz**, um Faktoren herauszuziehen.
4. **Nutze Abschätzungen**, falls eine exakte Lösung nicht notwendig ist (z. B. für Big-O-Notation). 
