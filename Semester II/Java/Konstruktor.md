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