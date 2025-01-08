# <font color = "orange">Views</font>
>[!INFO] Definition
>Eine View ist eine benutzerdefinierte Ansicht, die lokal auf einem Computer gespeichert wird. Sie erlaubt zudem eine spezifische Auswahl der Daten, sodass nur die Daten angezeigt werden, die die View anfordert.

>[!STRENGTHS]
>- Kompakte Darstellung und Vermeidung komplexer Abfragen
>- Automatische Verknüpfung verschiedener Tabellen
>- In DBMS vordefinierte und so optimierte, beschleunigte Abfragen
>- Stabilere Schnittstelle 

## Anlegen von Views
```
CREATE VIEW <viewname> [(spaltennamen)] AS <abfrage>
```
*abfrage* ist dabei eine beliebige Abfrage, die wie ein [[SELECT]]-Statement funktioniert.

>[!WARNING] *[[ORDER BY]]* darf jedoch nicht in Views verwendet werden.

>[!EXAMPLE] 
>```
>CREATE VIEW Leichtteile AS 
>SELECT TeilNr, Bezeichnung, Material, Gewicht 
>FROM Teile 
>WHERE Gewicht < 10 ;
>```

## Löschen von Views
```
DROP VIEW <viewname>
```
