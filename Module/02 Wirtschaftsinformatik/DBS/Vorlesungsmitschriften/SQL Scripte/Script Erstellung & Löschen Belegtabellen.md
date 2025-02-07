# <font color = "orange">Script Erstellung & Löschen Belegtabellen</font>
```
-- Tabelle "Belege" erstellen
CREATE TABLE Belege (
    Belegnummer NUMBER PRIMARY KEY,
    Belegtext VARCHAR2(100),
    Betrag NUMBER
);


-- PL/SQL-Block für die Belegerstellung
DECLARE
    n NUMBER := 50; -- Setze hier den gewünschten Wert für n
BEGIN
    FOR i IN 1..n LOOP
        IF MOD(i, 1) = 0 THEN -- Prüfe auf ungerade Zahl
            INSERT INTO Belege (Belegnummer, Belegtext, Betrag)
            VALUES (
                i, 
                'Beleg ' || TO_CHAR(i), 
                100 + 20 * i
            );
        END IF;
    END LOOP;
    COMMIT; -- Transaktion bestätigen
END;
/

DELETE FROM belege where belegnummer > 100 && < 500;

DELETE FROM Belege
WHERE Belegnummer BETWEEN 100 AND 500;

DELETE FROM Belege
WHERE Belegnummer = 38;

COMMIT; -- Änderungen bestätigen (wichtig bei manuellen Transaktionen)

DELETE FROM belege;
```
