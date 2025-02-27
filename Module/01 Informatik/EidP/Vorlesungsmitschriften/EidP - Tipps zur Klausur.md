# <font color = "orange">EidP - Tipps zur Klausur</font>
- Gibt ein neues Beispiel zu rekursiver Induktion in Racket 
    
- Beispiele sind im Moodle-Kurs verfügbar 
    
- Wenn wir alle Aufgaben fertig machen, dann können wir ihm die schicken und bekommen dann explizit zu unserer Lösung Feedback 
    
- Funktionen höherer Ordnung werden einen Teil der Klausur bestimmen, aber nicht zu viel 
    
- In der Klausur kommen ALLE Aufgabentypen dran 
    
- Aufgabe 23 und 24 a-f sollten wir machen, um für die Klausur bei  
    
- Bei Aufgabe 17 haben wir eine Aufgabe nicht besprochen. Wir sollten uns 17f ansehen. AUF JEDEN FALL ANSEHEN. GANZ WICHTIG. FLATTEN. 
    
- Statt Lambda auszuschreiben, können wir auch einfach das lambda-symbol machen. 
    
- Wir können uns auch ein check-expect abkürzen, indem wir einfach in der nächsten Zeile an der Stelle " machen 
    
- Wir können mit … abkürzen, wenn wir bei einer Auswertung den nicht relevanten Teil haben. 
    
- Wir können uns auch selbst Abkürzungen definieren, aber wir müssen halt überlegen, ob er das so verstehen kann. 
    
- Schließende Klammern sind eher irrelevant, Öffnende Klammern sind relevant. 
    
- Wir müssen an mindestens einer Stelle eine Funktionsschablone aufschreiben 
    

- Eine Schablone ist ein Racket-Ausdruck, bei dem durch … angedeutet wird, dass etwas eingesetzt werden muss, damit die Funktion funktioniert. 
    

(define f 

(lambda  [lvz …] 

(cond 

[(empty? Lvz) …] 

[else … (first lvz) … 

… (f (rest lvz) …) … ])))