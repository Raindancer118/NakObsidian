# <font color = "orange">Assembler-Code</font>
>[!INFO] Definition
>Hochsprachen werden vor ihrer Verarbeitung durch den [[Computer]] in Assembler-Code übersetzt, von wo aus sie weiter in Maschinencode übersetzt werden, die wiederum die CPU von Computern verarbeiten kann.

## Instruktionsarten
### Sprünge
>[!HOWTO] **Unbedingte** Sprünge
>Unbedingte Sprünge sind Sprünge, die durch eine Speicheradresse und nichts weiter definiert werden.
>`JMP target` - Programmausführung wird an 

>[!HOWTO] **Berechnete** Sprünge
>Berechnete Sprünge sind Sprünge, die durch eine Berechnung stattfinden. Beispielsweise könnte zur Adresse 2+*R1* gesprungen werden.

>[!HOWTO] **Bedingte** Sprünge
>Bedingte Sprünge sind kombinierte Sprünge, die aus den ersten beiden Arten und einer Bedingung gebildet werden.

>[!HOWTO] **Unterprogramm**-Aufrufe
>Diese Sprünge rufen über einen Sprung ein Unterprogramm auf und kehren anschließend wieder zur Ausgangsadresse zurück.
### Flags
Es können verschiedene Flags im **Statusregister** gesetzt werden. Dies hilft dabei, bestimmte Vorkommnisse zu unterschieden.
>[!HOWTO] **Negativ**-Flag
>Die Negativ-Flag wird gesetzt, falls das Ergebnis einer Rechenoperation negativ ist.

>[!HOWTO] **Overflow**-Flag
>Die Overflow-Flag wird gesetzt, falls das Ergebnis den möglichen Zahlenbereich über- oder unterschreitet.

>[!HOWTO] **Carry**-Flag
>Die Carry-Flag wird gesetzt, um den Übertrag der Addition zu transportieren.

>[!HOWTO] **Zero**-Flag
>Die Zero-Flag wird gesetzt, um zu markieren, dass das Ergebnis Null ist.

### Simple Befehle
**Rechenoperationen**
`ADD R1, #4` - **Addieren** zweier Zahlen (Hier: Den Inhalt von R1 + 4)
`SUB R1, R2` -  **Subtrahieren** zweier Zahlen (Hier: Den Inhalt von R1 - R2)
`CMP R1, R2` - **Vergleichen** zweier Zahlen
`INC R1` - **Erhöhen** von einer Zahl um 1
`DEC R1` - **Decrementieren** einer Zahl um 1
`NOT R1` - **Negation**, wobei der Inhalt der Speicherzelle mit dessen negierten Gegenpart überschrieben wird.
`XOR R1, R2` - **XOR**-Operation
`AND R1, R2` - **AND**-Operation
**Verschieben von Daten**
`MOV R1, R2` - Verschieben von Daten von R2 nach R1
`LOAD R1, [R2, offset]` - Ein Wert wird aus R2 + offset abgelesen und in R1 abgelegt.
`STORE [R2], R1` - R1 wird an Andresse R2 im Speicher abgelegt.
**Aufrufe von Unterprogrammen**
`CALL unterprogramm` - Ein Unterprogramm aufrufen
`RET` - Unterprogrammaufruf beenden und zurückkehren.

