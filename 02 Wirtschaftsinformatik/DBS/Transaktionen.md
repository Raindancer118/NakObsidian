# <font color = "orange">Transaktionen</font>
>[!INFO] Definition
>Eine Transaktion besteht aus mehreren Schreibvorgängen, die miteinander zu tun haben. Dabei müssen alle Transaktionen durchgeführt werden, oder es darf keine passieren.
>Falls eine der Buchungen nicht durchgeführt wird, wird ein sogenannter **Rollback** ausgeführt, sodass die bisherigen Schreibzugriffe der Transaktion nicht durchgeführt werden.

Bei einer Transaktion sollten die [[ACID-Eigenschaften]] eingehalten werden.