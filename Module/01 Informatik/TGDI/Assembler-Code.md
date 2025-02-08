# <font color = "orange">Assembler-Code</font>
>[!INFO] Definition
>Hochsprachen werden vor ihrer Verarbeitung durch den Computer in Assembler-Code übersetzt, von wo aus sie weiter in Maschinencode übersetzt werden, die wiederum die CPU von Computern verarbeiten kann.

## Instruktionsarten
### Sprünge
>[!HOWTO] **Unbedingte** Sprünge
>Unbedingte Sprünge sind Sprünge, die durch eine Speicheradresse und nichts weiter definiert werden.

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

