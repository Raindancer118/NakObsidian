# <font color = "orange">CONSTRAINT</font>
>[!INFO] Definition
>Constraints erlauben das Festlegen von Bedingungen für Manipulationen. Diese werden vor der Änderung überprüft. Dies ist für jede schreibende Änderung der Datenbank gültig.

Der Wert im Constraint muss immer angegeben werden. Dabei darf er nicht als `NULL` festgelegt werden. 

Constraints können als Spalten- oder auch Tabellen-Constraints angelegt werden.

## CONSTRAINTS ANLEGEN
```
[CONSTRAINT <name>] <bedingung>
<bedingung> := CHECK (<boolsche_bedingung>)
```

## Foreign-Key-CONSTRAINTS
Es gibt die Möglichkeit, eine Tabelle so einzustellen, dass automatisch Reaktionen durchgeführt werden, wenn die Zeile des Foreign-Keys gelöscht wird.
Dabei gibt es vier Optionen:
- `ON DELETE CASCADE`
	*Diese Option bietet die Möglichkeit, die Zeilen schlicht zu löschen.*
- `ON DELETE RESTRICT`
	*Diese Option ist bei ORACLE Standard. Es wird eine Fehlernachricht ausgegeben, falls versucht wird, einen Eintrag zu löschen, auf den ein Foreign-Key zeigt.*
- `ON DELETE SET NULL`
	*Diese Option setzt den Wert, von dem der Foreign-Key ausgeht, auf 0, falls das Ziel gelöscht wird.*
- `ON DELETE SET DEFAULT`
	*Diese Option setzt den Wert, von dem der Foreign-Key ausgeht, auf einen Standard-Wert. Dies könnte genutzt werden, um beispielsweise einen Wert zu hinterlegen, der anmerkt, dass das Ziel der Verknüpfung gelöscht wurde.*

>[!HOWTO] `ON DELETE`-Statements löschen
>`ON DELETE`-Statements können gelöscht werden, indem dafür ein [[DDL#^3a9948|ALTER TABLE <tabellenname> DROP]] verwendet wird.

