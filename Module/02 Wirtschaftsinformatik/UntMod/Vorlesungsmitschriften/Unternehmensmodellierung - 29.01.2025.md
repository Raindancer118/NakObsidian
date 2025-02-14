# <font color = "orange">Unternehmensmodellierung - 29.01.2025</font>
## BPMM Reifegradmodell
Ein BPMM Reifegradmodell wurde von der OMG entwickelt, von der *Object Management Group*. Es gibt dabei verschiedene Stufen der Reife in einem [[Unternehmen]].
1. Initial - Keine Struktur
2. Managed - Prozesse existieren auf Arbeitsebene und ein Process Management ist vorgesehen
3. Standardized - Prozesse sind standardisiert und [[Arbeitnehmer|Mitarbeiter]] haben [[Prozess]]-Know-How
4. Predictable - Prozessergebnisse und -Performance liefern vorhersagbare Ergebnisse und werden gesteuert
5. Innovating - Prozesse werden proaktiv gesteuert, innoviert und kontinuierlich verbessert und erfüllen interne und externe Anforderungen, Change Management
Es ist nicht unbedingt immer absolut sinnvoll, immer den höchsten Reifegrad für **jeden** [[Prozess]] zu erreichen. 
Bestimmte Aufgaben erfordern Kreativität und Flexibilität. 
Permanente, organisatorische Veränderungen können das [[Unternehmen]] in Schwierigkeiten bringen.

## Gateways in der Prozessmodellierung
### XOR (Datenbasiertes exklusives Gateway)
Vor dem Gateway muss eine Aktivität stehen, die eine Datengrundlage für das Routing des Gateways bietet.
Das XOR-Gateway kann Pfade auseinanderleiten, aber auch wieder zusammenführen.
>[!WARNING] Beim exklusiven Gateway trifft der Prozess selbst die Entscheidung, welcher Weg gegangen wird.
### (AND) Paralleles Gateway
**Alle** Pfade des AND-Gateways müssen durchlaufen werden und können durch ein weiteres AND-Gateway wieder synchronisiert werden. 
>[!WARNING] Parallel heißt nicht zeitgleich.

Das AND-Gateway kann allerdings auch parallel durchgeführt werden.

Wir haben am Ende der Vorlesung ein [Prozessdiagramm für Global Bike](https://academic.signavio.com/p/editor?id=e8946f3b8d7a4a0e91af4cdc5a82bba1) in [[SAP Signavio|Signavio]] erstellt.
### Komplexes Gateway
Eine Zusammenführung eines Gateways, das nicht vorher auseinanderging, kann in einem komplexen Gateway zusammengeführt werden. Es sollte immer eine Annotation am Rande zum Komplexen Gateway geben.