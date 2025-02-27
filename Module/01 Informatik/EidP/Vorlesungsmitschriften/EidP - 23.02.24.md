# <font color = "orange">EidP - 23.02.24</font>
Faustformel für das Auswerten von Ausdrücken: 

- Vereinfachung des äußersten und am weitesten links stehende Teilausdrucks 
    

Durch Testen kann man stets nur die Anwesenheit, nie aber die Abwesenheit von Fehlern beweisen. 

- Edgar W. Dijkstra 

Wenn wir die Korrektheit einer Funktion beweisen wollen, muss unser Programm formal korrekt sein und die formale Semantik des Ausdrucks muss korrekt sein. 

Wir können einen Beweis durch die vollständige Induktion über die Rekursionstiefe führen. 

Vollständige Induktion: Wir suchen uns irgendwo einen Dominostein in einer Reihe und kippen ihn um. Wir beweisen also, dass ein Stein an beliebiger Stelle dafür sorgt, dass die gesamte Reihe umkippen kann. 

Zustandlos heißt, dass wir nur eine Funktion haben, aber nichts irgendwo ablegen und nicht speichern. Wir führen etwas aus und wir nutzen sie immer wieder und wir verwenden vor allem keine Variablen. 

 Beweis mittels rekursiver Induktion: 

1. Behauptung 
    
2. Verankerung 
    

Beweis: 

Der Aufruf (len'()) liefert nach dem Ersetzungsmodell:  

(len '()) 

=((lambda [1st] 

(cond 

[(empty? 1st) 0] 

[else (+ 1 (len (rest 1st)))])) '()) 

= (cond 

[(empty? '()) 0] 

[else (+ 1 (len (rest '())))])) 

= (cond 

[#true 0 

[else (+ 1 (len (rest '())))]) 

= 0 

Beweis mittels vollständiger Induktion: 

Behauptung:  

Der Aufruf … liefert …  

Verankerung (Induktionsanfang): 

Wir zeigen, dass die Behauptung bei einer Rekursionstiefe von K = 0 gilt. 

K = 0, wenn … 

Annahme (Induktionsvoraussetzung): 

Die Behauptung gilt für eine Rekursionstiefe K = m, d.h. … 

Induktionsschluss (Induktionsschnitt): 

Es ist zu zeigen, dass der Aufruf … m+1 … den Wert liefert. 

Wenn wir zeigen können, dass wir die Induktion verstanden haben und zeigen, dass wir etwas in Racket beweisen können. 

Für die Klausur können wir uns merken, dass pro Minute ein Punkt zu holen ist. 

Mit let können Zwischenergebnisse gespeichert werden. 

(let [ (x 2) 

(y 3)] 

Damit sind also x und y gespeichert. 

let macht es auch möglich, Variablen zu überschreiben. 

Es gibt jetzt die Möglichkeit, rekursive Aufrufe auf Zeit zu machen. 

Wenn der letzte Ausführungsschritt ein rekursiver Funktionsaufruf ist, heißt die Funktion endrekursiv.