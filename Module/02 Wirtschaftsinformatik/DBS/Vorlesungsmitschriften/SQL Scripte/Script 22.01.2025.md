# <font color = "orange">Script 22.01.2025</font>
```
SET SERVEROUTPUT ON;

SELECT MAX(belegnummer) - count(belegnummer)-1 from belege;

DECLARE
    CURSOR findProblems_Cur IS
        SELECT * FROM belege
        ORDER BY belegnummer;
    lastnumber INTEGER := 0;
    startnumber INTEGER := 0;
    endnumber INTEGER := 0;
BEGIN
    dbms_output.put_line('Bitte prüfen Sie folgende Belege: ');
    
    FOR i IN findProblems_Cur
    LOOP
        IF i.belegnummer > lastnumber + 1 THEN
            startnumber := lastnumber + 1;
            endnumber := i.belegnummer - 1;
            FOR n IN startnumber..endnumber
            LOOP
                dbms_output.put_line(n);
            END LOOP;
        END IF;
        
        lastnumber := i.belegnummer;
    END LOOP;
END;
```