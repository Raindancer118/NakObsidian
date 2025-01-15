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

## Abort Befehl
>[!INFO] 
>Mit dem `abort`-Befehl lässt sich eine Transaktion bewusst durch den Nutzer abbrechen. Es wird dann explizit ein Rollback durchgeführt.