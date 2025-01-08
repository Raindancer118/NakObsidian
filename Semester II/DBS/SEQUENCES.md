---
aliases:
  - Sequence
---
# <font color = "orange">SEQUENCES</font>
>[!INFO] Definition
>Eine Sequence erlaubt das automatische Hochzählen eines Zählers, sodass beispielsweise immer eine eindeutige ID generiert wird, wenn ein neuer Eintrag angelegt wird.

```
CREATE SEQUENCE <seq_name>
	[INCREMENT BY <integer>]
	[START WITH <integer>]
	[MAXVALUE <integer> | NOMAXVALUE]
	[MINVALUE <integer> | NOMINVALUE]
```

>[!EXAMPLE]
>```
>CREATE SEQUENCE seq_KundenNr 
>INCREMENT BY 1 
>START WITH 1000 
>NOCYCLE;
>```

>[!HOWTO] Aktuellen Wert erhalten
>`<seq_name>.currval`

>[!HOWTO] Nächsten Wert erhalten
>`<seq_name>.nextval`

