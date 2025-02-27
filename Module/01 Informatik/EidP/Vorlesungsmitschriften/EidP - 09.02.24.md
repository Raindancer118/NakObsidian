# <font color = "orange">EidP - 09.02.24</font>
Racket kann nicht numerische Daten verarbeiten wie zb 

Symbole 

- Self-evaluating expressions 
    
- Atomare Daten 
    
- Wenn ich ein Hochkomma vor einer Variable einfüge wie zb 'symbol, dann ist das keine Variable, sondern etwas anderes, was dargestellt wird. Wenn 'symbol ausgewertet wird, wird wieder 'symbol ausgegeben. 
    

- Bilder 
    
- Töne 
    

Man kann Symbole über equal? auf Gleichheit überprüfen. 

"S" in "S-Ausdrücke" steht für "symbolischer Ausdruck" 

Alles, was sich zu sich selbst auswertet, ist ein Atom 

Ein S-Ausdruck kann eine Folge von S-Ausdrücke sein, die in runde Klammern eingeschlossen werden. Dazu gehören auch Listen. 

Racket basiert auf symbolischen Ausdrücken und eigentlich ist in Racket alles eine Liste. 

Ich kann eine leere liste einfügen, indem ich entweder '() mache oder empty schreibe 

Mit cons fügt man Elemente einer Liste zu 

(cons 'Karl empty) 

(cons 'Rosa (cons 'Karl empty) 

;; => (Rosa Karl) 

Cons fügt immer den neuen Ausdruck an den Anfang der Liste. 

Cons erwartet 2 Operatoren (Start und Ende) 

Wenn man Elemente hinzufügt, fügt man das immer vorne ran. Bspw: 

(cons 'Rosa (cons 'Karl (cons 'Michel empty))) 

Wenn ich das erste Element einer Liste haben möchte: 

(first (cons elem liste)) 

(Rest (cons elem liste)) => liste 

Wie kriege ich das zweite Element einer Liste? 

(rest (first (cons elem liste))) 

'(1 2 3 4 5 6)  

ist auch eine Liste 

Man kann einer Liste einen Namen geben mit define. 

(rest liste) 

> (list 2 3 4 5) 

Eine Liste ist entweder leer oder nicht leer. 

Eine leere Liste kann mit empty? erkannt werden. Eine andere Liste kann mit cons? erkannt werden. 

Einfach ein Test mit einer leeren Liste einfügen; sonst gibt’s Punktabzug 

Aufgabe 16: Werten sie die folgenden Funktionsausdrücke aus: