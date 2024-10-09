#### <font color = "orange">Wieso den Fermat-Test.?</font>
Der Fermat-Test bestimmt, ob eine Zahl $n$ eine Primzahl ist, oder nicht. Dies ist gerade für die Kryptologie, wo Primzahlen essentiell für die Verschlüsselung sind, sehr relevant.
#### <font color ="orange">Funktionsweise</font>
>[!INFO]
>**Step-By-Step-Anleitung**
>**1.** Wähle eine Zahl $a$, die größer als 1, aber kleiner als $n$ ist.
>**2.** Ist der ggT von $a$ und $n$ *nicht* 1, dann ist ***n keine Primzahl***
>**3.** Ist $a$<sup>(n -1)</sup> mod $n$ *nicht* 1, dann ist n ***keine Primzahl***
>
>**Übersteht *n* diese Tests, ist n *wahrscheinlich* eine Primzahl.**

>[!TIP]
>Die Wahrscheinlichkeit, dass **$n$ *trotz positivem Test* keine Primzahl ist, liegt bei $1/2$.
>Um sie zu senken, **führe den Fermat-Test iterativ immer wieder aus.**
>So kommt eine Fehlerwahrscheinlichkeit von $(1/2)$<sup>k</sup> heraus.

#crypto #primzahltest #DMII #primzahl