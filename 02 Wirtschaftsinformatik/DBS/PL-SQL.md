# <font color = "orange">PL/SQL</font>
>[!INFO] Definition
>PL/SQL steht für **P**rocedural **L**anguage **S**ystem **Q**uery **L**anguage. PL ist dabei ein Aufsatz, der Funktionen aus klassischen Programmiersprachen in SQL einbindet.

>[!STRENGTHS] 
>PL/SQL erlaubt die Ausführung von Skripts auf dem Server, sodass diese vorher an den Server übertragen und anschließlich in einem Block ausgeführt werden. 
>
>Zudem lassen sich Datenbankenabfragen und Skripte nun benennen, sodass diese per Schnellzugriff verfügbar sind. Ferner sind diese Unterprogramme weiter verwendbar, wie Methoden in Java, quasi.

## Befehle
>[!INFO] `BEGIN`
>Der Befehl `BEGIN` wechselt von SQL-Anweisungen in den PL/SQL-Modus, sodass die neuen Anweisungen ausgeführt werden können.

>[!INFO] `DECLARE`
>Der Befehl `DECLARE` erlaubt die Definition von Variablen oder benutzerdefinierten Exceptions.

>[!INFO] `END;`
>Der Befehl `END;` beendet die Ausführung von PL/SQL-Befehlen im Code und wechselt zurück zu normalem SQL.

>[!INFO] `EXCEPTION`
>Der Befehl `EXCEPTION` erlaubt das Abfangen von bestimmten Fehlern.
>
## Blocktypen
>[!INFO] Anonymer Block
>```
>[DECLARE]
>
>BEGIN
>	- statements
>[EXCEPTION]
>
>END;
>```

>[!INFO] Prozedur
>```
>PROCEDURE name
>IS
>
>BEGIN
>	- statements
>
>[EXCEPTION]
>END;
>```

>[!INFO] Funktion
>```
>FUNKTION name
>RETURN datatype
>IS
>BEGIN
>	- statements
>RETURN value
>[EXCEPTION]
>END;
>```
## Ausgabe von Textzeilen auf dem Bildschirm
Zunächst muss für die Ausgabe von Text auf dem Bildschirm der Befehl `SET SERVEROUTPUT ON` ausgeführt werden, um diese zu aktivieren.
## Variablen
Variablennamen dürfen eine Länge von maximal 30 Zeichen haben und dürfen Sonderzeichen, sowie Buchstaben und Zahlen enthalten. Sie dürfen nicht nach einem reservierten Ausdruck wie `SELECT` verwendet werden.
[[11_PLSQL v2.0jh.pdf#page=10|Siehe Folien für weitere Informationen]]

