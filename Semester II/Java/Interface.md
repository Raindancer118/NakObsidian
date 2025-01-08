---
aliases:
  - Interfaces
---
## <font color = "orange">Interface</font>

>[!SUMMARY]
>Ein Interface macht [[Klasse|Klassen]] im Endeffekt vergleichbar und ermöglicht es einer [[Methode]], mit einem statt mehreren [[Datentypen]] zu arbeiten und dennoch durch [[Vererbung|Mehrfachvererbung]] und [[Lose Kopplung|loser Kopplung]] verschiedene Objekttypen anzusprechen.

>[!WARNING] **ACHTUNG**
>Interfaces müssen [[Implementierung|implementiert]] werden. Hat eine [[Klasse]] ein Interface implementiert, muss sie **alle** [[Methode|Methoden]] daraus verwenden!

>[!HINT]
>Interfaces werden benannt, indem ein **"I" vor den Namen des [[Java - Datentyp|Datentyps]] gehängt wird, der verarbeitet werden soll**.

>[!INFO]
>Interfaces unterscheiden sich von [[Abstrakte Klasse|Abstrakten Klassen]] dadurch, dass Interfaces einen Schnittstellenvertrag bilden, der den [[Klasse|Klassen]] vorgibt, welche [[Methode|Methoden]] sie zu implementieren haben, aber nicht genau, wie. So machen Interfaces [[Klasse|Klassen]] vergleichbar und [[polymorph]].

>[!WARNING]
>Interfaces **können KEINE [[Exemplarvariable|Exemplarvariablen]] haben.** Interfaces können nur [[Konstante|Konstanten]] haben, also [[Programmierung - Variable|Variablen]] mit den Modifikatoren **public static final**.

>[!EXAMPLE]
>*public interface IPost{
>...
>}*
