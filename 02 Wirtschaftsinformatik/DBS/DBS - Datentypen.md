---
aliases:
  - Datentypen
  - Datentyp
---
# <font color = "orange">SQL Datentypen</font>
>[!INFO] Definition
>SQL benötigt bestimmte Datentypen, in denen Daten zu speichern sind. Diese sind hier aufgelistet, allerdings mit einem Blick auf ORACLE [[Datenbanken]].

### Ganze Zahlen
- SMALLINT
- INTEGER
- BIGINT
### Festkommazahlen
- DECIMAL / NUMERIC
### Gleitkommazahlen
- FLOAT
- REAL
- DOUBLE PRECISION
### Texte
- CHAR(q)
- VARCHAR(q)

>[!WARNING] q bedeutet bei CHAR die **genaue Anzahl** und bei VARCHAR die **maximale Anzahl von Zeichen**.
### Zeiten / Daten
- DATE
- TIME
### Große Datenmengen
- CLOB
	*CLOB steht dafür für **C**haracter **L**arge **OB**ject*.
- BLOB
	*BLOB steht dafür für **B**inary **L**arge **OB**ject*.
### Andere Datentypen
Es ist möglich, in [[Datenbanken]] andere Datentypen zu definieren. Dabei muss allerdings aufgepasst werden, dass nicht gegen die [[Normalformen#1. Normalform|1. Normalform]] verstoßen wird.

# <font color = "orange">PL/SQL Datentypen</font>
## Zusammengesetzte Datentypen
Zusammengesetzte Datentypen erlauben die Speicherung 