# <font color = "orange">EidP - 01.03.24</font>
Wir zeigen, dass die Behauptung bei einer Rekursionstiefe von k=0 gilt. (f 0) besitzt Rekursionstiefe 0 und liefert nach dem Ersetzungsmodell: 

(siehe Notizen) 

I.V. 

Die Behauptung gilt für eine Rekursionstiefe k=m, d.h. (f m) = m/(m+1)   (K = m, wenn n = m). 

I.S.: Wir zeigen, dass mit der Annahme auch die Behauptung für k = m + 1 gilt. --> k = m + 1 wenn n = m +1. 

Es ist zu zeigen, dass der Aufruf (f (+ m 1)) den Wert (m+1)/(m+2) als Resultat liefert. 

Option: 

Sei x = (+ m 1)  -> Wir können uns Ausdrücke, die wir oft schreiben müssen, als Variable speichern, damit wir sie nicht immer wieder schreiben müssen. 

Funktionen höherer Ordnung 

Wenn Funktionen über Lambda mitgegeben werden, werden sie zwar wie ein Wert mitgegeben, aber aufgerufen wie normal. 

Liste von Funktionen höherer Ordnung 

- Identity 
    
- Add1 
    
- Filter 
    

Wir können jetzt eine generische Funktion schreiben, die mehrere Zwecke gleichzeitig erfüllen kann 

Map 

- Damit kann man Funktionen zusammenfassen 
    

Fold 

- Addiert alle Elemente einer Liste