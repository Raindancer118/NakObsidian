# <font color = "orange">DDL</font>
>[!INFO] Definition
>DDL steht für **D**ata **D**efinition **L**anguage. Dabei ist dies die Sprache mit der neue Tabellen angelegt oder auch Tabellen gelöscht werden.

>[!HINT] Dieser Teil der Vorlesung wird in [[09_SQL_DDL v2.0jh.pdf]] besprochen.

## Erstellen von Tabellen
```
CREATE TABLE <tabellenname> (<attributsname> <datentyp>, ..., <attributsname> <datentyp>) 
```

>[!EXAMPLE] Beispiel für die Kreation einer Tabelle
>```
>CREATE TABLE Verkaeufer ( Vnr INTEGER, Name VARCHAR(6), Status VARCHAR(7), Gehalt INTEGER, PRIMARY KEY (Vnr) );
>```

Die Zahlen in den runden Klammern hinter den Datentypen bedeuten in diesem Zusammenhang die maximale Anzahl Zeichen, die in dem jeweiligen Feld verarbeitet werden.
#### Tabellennamen
Tabellennamen dürfen maximal 30 Zeichen in Buchstaben und Zahlen beinhalten, sollten aber mit einem Buchstaben beginnen.

## Tabelleneigenschaften ändern
```
ALTER TABLE <tabellenname>
```

Hier gibt es verschiedene Optionen:
- `ADD <spaltenname> <datentyp>`
- `RENAME COLUMN <spaltenname> TO <neuerSpaltenname>`
- `DROP <PRIMARY KEY>`
	- `UNIQUE (<spaltenliste>)`
	- `CONSTRAINT <constraintname>`
	- `COLUMN <spaltenname>`
- `DISABLE <PRIMARY KEY>`
	- `UNIQUE (<spaltenliste>)`
	- `CONSTRAINT <constraintname>`
	- `ALL TRIGGERS`
- `ENABLE <PRIMARY KEY>`
	- `UNIQUE (<spaltenliste>)`
	- `CONSTRAINT <constraintname>`
	- `ALL TRIGGERS`
- `MODIFY <spaltenname> <datentyp>`

>[!HINT] `DROP` löscht die gesamte Tabelle, inklusive der Struktur, während `DELETE` nur die Daten innerhalb der Tabelle löscht.
