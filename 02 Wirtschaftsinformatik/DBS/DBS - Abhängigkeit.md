# <font color = "orange">Abhängigkeit</font>
>[!INFO] Es gibt grundsätzlich zwei Arten der Abhängigkeit zwischen Daten voneinander.
## Funktionale Abhängigkeit
Eine funktionale Abhängigkeit besteht, wenn von einem Attribut eindeutig auf ein anderes geschlossen werden kann. 
Angenommen, es gibt ein Objekt $A$ und dieses könnte durch die Nummer $B$ eindeutig identifiziert werden, dann wäre dieses $A$ **funktional abhängig** von $B$.
## Voll funktionale Abhängigkeit
Eine voll funktionale Abhängigkeit besteht dann, wenn alle Objekte $A$ benötigt werden, um $B$ eindeutig zu identifizieren. 
>[!EXAMPLE]
>PersonalNr. | ProjektNr. | Rolle
>-------------|-------------|------
>01 | P10 | Projektleiter
>01 | P24 | Projektmitarbeiter
>02 | P10 | Projektmitarbeiter
>
>In diesem Beispiel kann die Rolle eines Mitarbeiters nicht klar identifiziert werden, solange nicht sowohl Projektnummer als auch Personalnummer vorliegen. Dies liegt daran, dass ein Mitarbeiter in unterschiedlichen Projekten unterschiedliche Rollen haben könnte.

