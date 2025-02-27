# <font color = "orange">EidP - 19.01.24</font>
Aufgabe 2 

1. Die Funktion "(* (+ 2 2) (/ (* (+ 3 5) (/ 30 10)) 2))" wird aufgelöst zu 48. 
    
2. Siehe Wörterbuch 
    
3. Racket-Output: 
    

> (- 1.0 0.9) 

0.1 

> (- 1000.0 999.9)  

0.1 

> (- #i1000.0 #i999.9) 

#i0.10000000000002274 

Aufgabe 3 

(define a (lambda [n] (+ (sqr n) 1))) 

(define b (lambda [n] (+ (sqr (/ n 2)) 3))) 

(define c (lambda [n] (- 2 (/ 1 n)))) 

Aufgabe 4 

1. (define Q (lambda [a b c](* a b c)))  
    

Normalerweise ist es in der Klausur so, dass die erste Aufgabe Multiple Choice ist und dass man dort 6 Punkte bekommt.  

- Funktionsaufrufe in Racket beginnen immer mit einer öffnenden Klammer 
    
- Racket ist ein Lisp-Dialekt 
    
- Es gibt in Racket Ausdrücke, die syntaktisch korrekt sind, deren Auswertung aber kein Resultat bietet. 
    
- Syntaktisch korrekte Sätze in einer Programmiersprache haben, genau wie natürliche Sprachen, keine eindeutige Semantik. 
    
- Programme und Daten, die auf einem handelsüblichen Computer verarbeitet werden sollen, müssen letzendlich binär vorliegen. 
    
- Self evaluating expressions sind Ausdrücke, die sich zu sich selbst auswerten.  
    

Grundsätzlich werden Funktionen in Racket wie folgt angegeben: 

(operator, operand1, operand2, operand3, …) 

Es ist nicht möglich, die Operation +2 auszuführen, daher  würde diese Schreibweise Probleme aufwerfen. 

Die eröffnenden Klammern müssen da sein. Ob wir jetzt rechts vier oder fünf Klammern haben, ist ihm egal. 

Zur Klausur bekommen wir die Regeln zum Aufschreiben von Funktionen 

Wenn er den Satz nicht lesen kann, dann gibt’s dafür keine Punkte. 

 Rechtschreibung wird allerdings nicht bewertet. 

In Racket wird alles klein geschrieben und mit Bindestrichen verbunden. 

Regeln 

- Verwende aussagekräftige Namen für Funktionen und Variablen ("sprechende Bezeichner"). 
    
    - Zb: (define endkapital) 
        
- Beschreibe den Zweck der Funktion durch einen Satz, der das Resultat der Funktion in Abhängigkeit von ihren Argumenten beschreibt. Diese Beschreibung sollte über den entsprechenden Block geschrieben werden. 
    
    - In den Kommentaren sollte man möglichst Fachbegriffe verwenden 
        
- Schreibe Beispielanwendung der Funktionen auf, die das Resultat der Funktion mit dem Erwartungswert vergleichen. Die Auswertung der Funktion muss dabei immer den Wahrheitswert #true liefern. Davon sollte es eigentlich mindestens drei geben, aber wir sollten die Aufgaben in der Klausur lesen, weil dort der Rest von Regel 3 stehen könnte. 
    
    - (= (endkapital 1000 0 24) 1000) 
        

Tests 

- Am Anfang werden Beispielanwendungen verwendet, um  
    

Gewinn = Umsatz - Ausgaben 

Profit = Einnahmen - Kosten 

Die Einnahmen in dem folgenden Beispiel bestimmten sich folgendermaßen: 

Kartenpreis * Besucherzahl 

Die Kosten bestimmten sich so: 

Fixkosten + Vorkosten * Besucherzahl 

f(x)=mx+b 

In diesem Fall:  

b(p) = 120-1,5*(p-500) 

Centangaben werden immer eher empfohlen als Euro-Angaben.