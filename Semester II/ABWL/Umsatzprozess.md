# <font color = "orange">Umsatzprozess</font>

Zunächst werden die für die Produktion benötigten Mittel auf dem [[Beschaffunsmarkt]] beschafft. Anschließend werden, wenn nötig, finanzielle Mittel vom [[Kreditmarkt]] gezogen, um diese für die Transformation zu nutzen.
Nach der Transformation kann schließlich das fertige Erzeugnis am [[Absatzmarkt]] verkauft werden. Die daraus entstandenen [[Einnahme|Einnahmen]] werden verwendet, um 
```mermaid
flowchart TD

    C[Beschaffungsmarkt]

    D[Absatzmarkt]

    E[Arbeitsleistung]

    C --> E

    F[Transformationsprozess]

    E --> F

    G[Halb- und Fertigfabrikate]

    F --> G

    G --> D

    H[Finanzielle Mittel]

    H --> |Ausgaben| C

    D --> |Einnahmen| H

    I[Kreditmarkt]

    I --> |Beschaffung von finanziellen Mitteln| H

    H --> |Rückzahlung von Krediten| I
```
