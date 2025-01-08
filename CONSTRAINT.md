# <font color = "orange">CONSTRAINT</font>
>[!INFO] Definition
>Constraints erlauben das Festlegen von Bedingungen für Manipulationen. Diese werden vor der Änderung überprüft. Dies ist für jede schreibende Änderung der Datenbank gültig.

Der Wert im Constraint muss immer angegeben werden. Dabei darf er nicht als `NULL` festgelegt werden. 

Constraints können als Spalten- oder auch Tabellen-Constraints angelegt werden.

## CONSTRAINT-SYNTAX:
```
[CONSTRAINT <name>] <bedingung>
<bedingung> := CHECK (<boolsche_bedingung>)
```

