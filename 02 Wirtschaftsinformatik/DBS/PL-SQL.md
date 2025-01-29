# <font color = "orange">PL/SQL</font>
>[!INFO] Definition
>PL/SQL steht für **P**rocedural **L**anguage **S**tructured **Q**uery **L**anguage. PL ist dabei eine Erweiterung für SQL, die Funktionen aus klassischen Programmiersprachen einbindet.
>
>Natürlich könnte man auch Datenbankenzugriffe über andere prozedurale Programmiersprachen durchführen, doch PL/SQL ist in der Performance stärker als diese Optionen.

>[!HINT] Dieser Teil der Vorlesung wird in [[11_PLSQL v2.0jh.pdf]] besprochen.

>[!STRENGTHS] 
>PL/SQL erlaubt die Ausführung von Skripts auf dem Server, sodass diese vorher an den Server übertragen und anschließlich in einem Block ausgeführt werden. 
>
>Zudem lassen sich Datenbankenabfragen und Skripte nun benennen, sodass diese per Schnellzugriff verfügbar sind. Ferner sind diese Unterprogramme weiter verwendbar, wie Methoden in Java, quasi.
## Befehle
>[!INFO] `BEGIN`
>Der Befehl `BEGIN` wechselt von SQL-Anweisungen in den PL/SQL-Modus, sodass die neuen Anweisungen ausgeführt werden können.

>[!INFO] `DECLARE`
>Der Befehl `DECLARE` erlaubt die Definition von [[Programmierung - Variable|Variablen]] oder benutzerdefinierten Exceptions.

>[!INFO] `END;`
>Der Befehl `END;` beendet die Ausführung von PL/SQL-Befehlen im Code und wechselt zurück zu normalem SQL.

>[!INFO] `EXCEPTION`
>Der Befehl `EXCEPTION` erlaubt das Abfangen von bestimmten Fehlern.
>

>[!HOWTO] `LOOP`
>Der Befehl `LOOP` erlaubt das Bauen einer Schleife à la `while` in Java. Zudem kann eine Bedingung für diesen Loop festgelegt werden.

>[!HOWTO] Kommentar
>Ein Kommentar kann mit zwei Minussen nacheinander geöffnet werden. Also so: `--`.
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
## [[Programmierung - Variable|Variablen]]
Variablennamen dürfen eine Länge von maximal 30 Zeichen haben und dürfen Sonderzeichen, sowie Buchstaben und Zahlen enthalten. Sie dürfen nicht nach einem reservierten Ausdruck wie `SELECT` verwendet werden.
[[11_PLSQL v2.0jh.pdf#page=10|Siehe Folien für weitere Informationen]]

## `%ROWTYPE`
Mithilfe von `%ROWTYPE` lässt sich die Struktur einer Tabelle komplett übernehmen, sodass Daten aus verschiedenen Spalten einfach in eine einzige Variable gespeichert werden können.
## Prozeduren
Prozeduren sind Funktionen, die definiert werden können. Wird ihnen einen Namen gegeben, dann werden diese vom Oracle-DBMS in kompilierter Form abgelegt und auf dem Server gespeichert und auch dort ausgeführt.
Trigger können dabei Prozeduren automatisch ausführen.
>[!INFO] Syntax
>```
>CREATE (OR REPLACE) PROCEDURE {Prozedurname}
>	[({parameterliste})] IS
>	{lokaleVariable}
>	BEGIN
>		{Prozedurrumpf}
>	END;
>```
### Trigger
Prozeduren können durch Trigger ausgelöst werden, die nach einem bestimmten Befehl oder einer bestimmten Aktion direkt eine Aktion durchführen. 
>[!INFO] Trigger erstellen
>```
>CREATE [OR REPLACE] TRIGGER >Triggername<
>```
#### FORMULA