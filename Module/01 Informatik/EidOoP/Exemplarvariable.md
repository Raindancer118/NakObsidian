---
aliases:
  - Exemplarvariablen
---
## <font color = "orange">Exemplarvariable</font>

>[!SUMMARY]
>Exemplarvariablen **bestimmen den [[Zustand]] eines [[Java - Objekt|Objektes]]** oder geben die Möglichkeit, **[[Java - Datentyp|Daten]] methodenübergreifend zu speichern**.

>[!HINT]
>Exemplarvariablen stehen **zwischen [[Klassenkopf]] und [[Konstruktor]]**. 
>Sie können entweder bereits [[Initialisierung|initialisiert]] oder auch nur [[Deklaration|deklariert]] sein.
>Die finale **[[Zuweisung]] findet meist im [[Konstruktor]] statt.**
>
>Besagte Zuweisungen funktionieren über **[[this.]]**, da die [[Parameter]] meist genauso heißen wie die Exemplarvariable.

>[!TIP]
>Wenn möglich, wird versucht, die **[[Sichtbarkeit]] von Exemplarvariablen auf Privat** zu halten und Ausgabe oder Setzen über [[Getter]]- und [[Setter]]-[[Methode|Methoden]] zu lösen.

>[!EXAMPLE]
>*public [[Klasse|class]] Apple{*
>
>**private [[String]] color;**
>
>*public Apple(String color){
>this.color = color;
>}*
