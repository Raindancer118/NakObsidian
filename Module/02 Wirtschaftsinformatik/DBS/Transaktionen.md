---
aliases:
  - Transaktion
  - Bearbeitung
---
# <font color = "orange">Transaktionen</font>
>[!INFO] Definition
>Eine Transaktion besteht aus mehreren Schreibvorgängen, die miteinander zu tun haben. Dabei müssen alle Transaktionen durchgeführt werden, oder es darf keine passieren.
>Falls eine der Buchungen nicht durchgeführt wird, wird ein sogenannter **Rollback** ausgeführt, sodass die bisherigen Schreibzugriffe der Transaktion nicht durchgeführt werden.
>Häufig werden die Transaktionen 

Bei einer Transaktion sollten die [[ACID-Eigenschaften]] eingehalten werden.

## Befehle
>[!INFO] `BEGIN TRANSACTION`
>Der Befehl `BEGIN TRANSACTION` startet eine Transaktion. Bei Oracle ist dies allerdings nicht notwendig.

>[!INFO] `COMMIT`
>Der Befehl `COMMIT` übernimmt die vorher eingegebenen Befehle endgültig als richtig in die Datenbank.

>[!INFO] `ABORT`
>Mit dem `abort`-Befehl lässt sich eine Transaktion bewusst durch den Nutzer abbrechen. Es wird dann explizit ein Rollback durchgeführt.

>[!INFO] `ROLLBACK`
>Der Rollback-Befehl macht Befehle bis zum letzten `COMMIT`-Befehl rückgängig.

>[!INFO] `SAVEPOINT`
>Der `SAVEPOINT`-Befehl ermöglicht das Speichern von Zwischenständen, sodass ein `ROLLBACK` nur bis zu diesem Punkt zurückrollt, statt bis zum letzten `COMMIT`. `SAVEPOINT`-Befehle lassen sich zusätzlich benennen.