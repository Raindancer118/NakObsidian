## <font color = "orange">Compiler</font>

>[!SUMMARY]
>Der Compiler übersetzt den menschengeschriebenen [[Quellcode]] in [[maschinenunabhängig|maschinenunabhängigen Bytecode]], sodass dieser von der [[JVM]] ausgeführt werden kann.
>Nebenbei prüft er den [[Quellcode]] auf [[Syntaxfehler]] und gibt diese zurück.

>[!INFO]
>Die Zeit **von dem Moment, ab dem der Compiler startet, bis zu dem, wo er den [[maschinenunabhängig|Bytecode]] an die [[JVM]] übergibt, nennt man [[Compilezeit]].

## <font color = "orange">Datentyp</font>

>[!SUMMARY]
>Daten von [[Variable|Variablen]] oder auch [[Parameter|Parametern]] besitzen einen bestimmten Typ. Damit [[Methode|Methoden]] wissen, welchen genau sie verarbeiten sollen, existieren Datentypen, die **vor der [[Variable]]** angegeben werden.

>[!IMPORTANT]
>**Datentypen:**
>1. [[String]]
>2. [[Integer]]
>3. [[Long]]
>4. [[ArrayList]]
>5. [[Array]]
>6. [[Interface]]
>7. [[Klasse|Class]]
>8. [[Char]]

## <font color = "orange">Exemplarvariable</font>

>[!SUMMARY]
>Exemplarvariablen **bestimmen den [[Zustand]] eines [[Objekt|Objektes]]** oder geben die Möglichkeit, **Daten methodenübergreifend zu speichern**.

>[!HINT]
>Exemplarvariablen stehen **zwischen [[Klassenkopf]] und [[Konstruktor]]**. 
>Sie können entweder bereits [[Initialisierung|initialisiert]] oder auch nur [[Deklaration|deklariert]] sein.
>Die finale **[[Zuweisung]] findet meist im [[Konstruktor]] statt.**
>
>Besagte Zuweisungen funktionieren über **[[this.]]**, da die [[Parameter]] meist genauso heißen wie die Exemplarvariable.

>[!TIP]
>Wenn möglich, wird versucht, die **[[Sichtbarkeit]] von Exemplarvariablen auf Privat** zu halten und Ausgabe oder Setzen über [[Getter]]- und [[Setter]]-[[Methode|Methoden]] zu lösen.

>[!EXAMPLE]
>*public class Apple{*
>
>**private [[String]] color;**
>
>*public Apple(String color){
>this.color = color;
>}*

## <font color = "orange">Frühe Bindung</font>

>[!SUMMARY]
>Frühe Bindung ist, wenn noch **vor der [[Compilezeit]]** klar ist, **für was die gegebene [[Methode]] ausgeführt wird**.

>[!EXAMPLE]
>Frühe Bindung ist, wenn man in den Supermarkt geht, mit dem Gedanken, Pizza zu kaufen.


## <font color = "orange">JRE</font>

>[!SUMMARY]
>**Die Java Runtime Environment (JRE) ist eine Softwareumgebung, die benötigt wird, um Java-Programme auszuführen.** Sie enthält alle notwendigen [[Klasse|Klassen]] und [[Bibliothek|Bibliotheken]], damit der von einem Java-[[Compiler]] erzeugte [[maschinenunabhängig|Bytecode]] interpretiert und ausgeführt werden kann. **Die JRE ist [[maschinenunabhängig|plattformunabhängig]] und ermöglicht es, Java-Anwendungen auf verschiedenen Betriebssystemen wie Windows, macOS und Linux ohne Neu [[Compiler|kompilieren]] zu müssen.**

## <font color = "orange">JVM</font>

>[!SUMMARY]
>Die JVM, auch **Java Virtual Machine**, ermöglicht, dass Java **[[maschinenunabhängig]] läuft**. Sie baut eine virtuelle Umgebung, das [[JRE]], in der das Programm als [[maschinenunabhängig|Bytecode]], nach der Übersetzung durch den [[Compiler]], laufen kann.
>
>**Die JVM ist ESSENZIELL für Java-Programme!**

## <font color = "orange">Konstruktor</font>
#### <font color="orange"> Syntax des Konstruktors </font>

> [!summary]
> Der Konstruktor ist eine spezielle Methode, die automatisch aufgerufen wird, wenn ein **neues [[Objekt]] einer [[Klasse]]** erstellt wird, um dieses **Objekt zu [[Initialisierung|initialisieren]]** und in einen **gültigen [[Zustand]] zu versetzen**.

```
sichtbarkeit klassenname (Parameter hier) {
// konstruktor-körper
}
```

**Beispiel in Java:**
```
public Apple() {
}
```

#### <font color = "orange"> Zuweisung von Exemplarvariablen</font>
Im Konstruktor können beispielsweise die [[Exemplarvariable]] auf durch [[Parameter]] mitgegebene Werte gesetzt werden. 
Dafür werden die Parameter des Konstruktors so gesetzt, dass diese bei der Erstellung eines [[Objekt|Objektes]] der [[Klasse]] mitgegeben werden müssen. Im Anschluss können sie über eine [[Zuweisung]] gespeichert werden.

**Beispiel:**
```
// Klassenkopf:
public class Apple{

// Exemplarvariablen:
private boolean halfEaten;
private int size;

// Konstruktor:
public Apple(boolean halfEaten, int size) {
// Zuweisung der Variablen innerhalb des Konstruktors:
this.halfEaten = halfEaten;
this.size = size;
}

...
}
```