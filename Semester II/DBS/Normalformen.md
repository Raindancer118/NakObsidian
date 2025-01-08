# <font color = "orange">Normalformen</font>
>[!INFO] Definition
>Die Normalformen sind unterschiedliche Regeln, die der Normalisierung und Funktionalität von [[Datenbanken]] dienen. 

>[!STRENGTHS] Vorteile der Einhaltung der Normalformen
>- Steigende **Qualität**
>- **Vermeidung von Anomalien & Redundanzen**
>- **Geringere Fehleranfälligkeit**
>- Korrektere **Abbildung der Realität**

>[!WEAKNESSES] Nachteile der Normalformen
>- **Höhere Komplexität**
>- Durch notwendige Zusammenführung evtl **Performance-Einbußen**
## 1. Normalform
Die erste Normalform gilt als erfüllt, wenn die Werte der Tabellen einer Datenbank ausschließlich in atomarer Form vorliegen, also **ein Wert pro Zelle**, nicht mehr.
## 2. Normalform
Die zweite Normalform gilt als erfüllt, wenn die Tabelle in [[#1. Normalform]] ist und zudem jeder Wert, der nicht als [[Schlüsselattribut]] fungiert, voll funktional von einem [[Schlüsselattribut]] abhängig ist.
>[!HOWTO] Wie?
>Zur Bildung der zweiten Normalform müssen Tabellen eventuell in mehrere Tabellen zerlegt werden, sodass nicht mehr mehrere Relationen in einer Tabelle aufgezeigt sind. 
>Siehe [[05_Normalisierung v2.0jh.pdf#page=12]]
## 3. Normalform
Die dritte Normalform gilt als erfüllt, wenn die Tabelle in [[#2. Normalform]] sind und zudem keine funktionalen Abhängigkeiten zwischen Nicht-[[Schlüsselattribut|Schlüsselattributen]] bestehen. 
>[!HINT] Normalerweise reicht es, Tabellen in dritter Normalform vorliegen zu haben.