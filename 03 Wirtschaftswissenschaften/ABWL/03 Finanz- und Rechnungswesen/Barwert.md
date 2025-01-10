# <font color = "orange">Barwert</font>
## Barwert
>[!summary]
>Der Wert, der einer Zahlung, die noch in der Zukunft liegt, heute zugemessen wird.
![[Pasted image 20241228091352.png]]

>[!INFO] **Definition**
>Der Barwert stellt dar, welcher Betrag gerade zu einem bestimmten Zinssatz angelegt werden müsste, um in einem gewissen Zeitraum die Summe einer zukünftigen Zahlung zu erreichen. 

>[!FORMULA]
>Die Berechnung funktioniert anhand der folgenden Formel:
>$$
>Z_0=Z_t\frac{1}{(1+i)^t}
>$$
>Dabei steht $i$ für den Prozentsatz der Zinsen, $Z_0$ für den Barwert und $Z_t$ für den Soll-Wert der Zahlung in der Zukunft. $t$ ist dabei die Anzahl der Jahre, die die Zahlung noch in der Zukunft liegt.

^a90d45

>[!EXAMPLE]
>Angenommen, der Soll-Wert einer Zahlung liegt bei $5000$€ und sie wird knapp zwei Jahre im Voraus bereits zu einem Prozentsatz von 6% angelegt. Dann ergibt sich folgende Rechnung:
>$$
>Z_0 = 5000\frac{1}{(1+0,06)^2}=4449,98\text{€}
>$$

>[!HINT] **Wenn vorhanden, nutze Abzinsungstabellen, um die Berechnung zu ersparen!**

---
## Rentenbarwert
>[!summary]
>Gibt den Barwert an für mehrere Konstante Zahlungen am Jahresende über n (gewisse Anzahl) Jahre an.
>![[Pasted image 20241228091411.png]]

>[!INFO] Definition
>Der Rentenbarwert ist quasi der **Barwert**, doch wird davon ausgegangen, dass über die Spanne der Jahre, die das Geld angelegt wird, Zahlungen mit dem Wert $Z$ ausgeführt werden.
>Theoretisch könnte nun repetitiv dieselbe Rechnung durchgeführt werden, sodass der Barwert für jedes Jahr erneut ausgerechnet wird.
>$$
>Z_0=Z\frac{1}{(1+i)^1}+Z\frac{1}{(1+i)^2}+\text{...} Z\frac{1}{(1+i)^n}
>$$

>[!FORMULA]
>Aus eben genannter Formel ergibt sich die **Formel für den Rentenbarwert**, die da wäre:
>$$
>Z_0=Z(\frac{(1+i)^n - 1}{i(1+i)^n})
>$$

^9d6089

## Abzinsen 

>[!summary]
>Der Vorgang zukünftige Zahlung auf einen Heutigen stand runterzurechnen. 
>Also wie viel wäre eine Zukünftige zahlung heute wert.
>Man berechnet so den [[Barwert]]