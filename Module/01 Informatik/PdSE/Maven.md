# <font color = "orange">Maven</font>
>[!INFO] Definition
>Maven wurde von der Apache [[Software]] Foundation veröffentlicht. Das Tool ermöglicht das Builden und die Dokumentation von Projekten. Dafür nutzt Maven pom.xml-Files.

Maven sieht eine Standard-Verzeichnisstruktur vor. Diese unterscheidet sich nicht stark von der Standard-Struktur von [[IntelliJ]].

## POM-Files
>[!HINT] **POM steht für *Project Object Model***.

Ein Maven-Projekt benötigt keinen [[Quellcode]]; ausschließlich eine pom.xml-Datei.
Die POM-Datei bietet sehr viele Konfigurationsmöglichkeiten. Die ohnehin schon große Funktionalität kann weiter erweitert werden durch Plugins. 
Eine POM-Datei beinhaltet:
- [[Dependency|Dependencies]]
- Identifikatoren (Eindeutige IDs für das Projekt)
- Zugehörigkeit zu anderen POM-Files
- Enthaltene Module
- Eigenschaften ([[JRE]])
- [[Building|Build]] Einstellungen
- Weitere Projektinformationen
- Umgebungseinstellungen

Das Testen kann Teil des Buildings sein, sodass ein tatsächlich finaler [[Building|Build]] ohne erfolgreiche Testphase gar nicht erst funktioniert.
### XML/Modell Einstellungen
In der Vorlesung wird fix `modelVersion 4.0.0` verwendet.
### Metadaten
- groupId: Eine GroupId sollte mit dem Pfad des Projektes auf dem Datenträger korrespondieren, muss aber nicht "C:\\" und so sein.
- artifactId: Der offizielle Name des Projektes
- version: die Version der [[Software]], damit man identifizieren kann: groupId:artifactId
- type: .jar oder .war
- scope:
- optional: Erklärt, ob die [[Dependency]] zwangsweise zum [[Building|Bauen]] des Projektes verfügbar sein muss, oder ob es auch ohne dieses Projekt funktioniert.
- [[Dependency|dependencies]]: auch die [[Dependency|Dependencies]] werden diesem Schema nach aufgeschrieben.
### Plugins
`plugins` beinhaltet Details zu Apache Plugins, in denen bspw das Maven-Jar-Plugin eingefügt werden kann. Dieses findet sich unter *MVN Repositories*.
### Reporting
Maven kann über Plugins nach dem [[Building|Build]] anzeigen lassen, was für Vulnerabilities der Code beinhaltet. Dies läuft in einem eigenen Verzeichnis und lässt sich ebenfalls in der POM-File regeln.
Reports lassen sich bilden über beispielsweise das Plugin *maven-projekt-info-reports*.

## Kommandozeilen-Befehle
`mvn verify` ist der Befehl der normalerweise zum Builden des Projektes ausreicht.
`mvn clean verify` ist die Alternative, bei denen zunächst "aufgeräumt" wird.

## Maven Lifecycle
Maven's [[Building|Build]] Lifecylce
### Maven Clean Lifecycle
Hier werden die Daten des vorangegangenen Builds gelöscht.
Es gibt drei Unter-Phasen:
- pre-clean
- clean - hier werden alle Dateien der vorangegangen Builds gelöscht.
- post-clean
Der [[Building|Build]]-Prozess könnte beschleunigt werden, wenn 
### Maven Default Lifecycle
Besteht grob aus 23 Phasen
- **[[validate]]**
- **[[initialize]]**
- **generate-sources**
- **generate-resources**
- **[[compile]]**
- **generate-test-sources**
- **generate-test-resources**
- **test-[[Compiler|compile]]**
- **test** - hier werden Tests durchgeführt, über bspw jUnit Tests.
- **pre-[[Packages|package]]**
- **pre-integration-tests** - Integrationstests; es wird geprüft, ob sich die [[Software]] mit anderen Komponenten integrieren lässt.
- **[[verify]]**
- **[[install]]** - Ablegen des Artefaktes in das lokale Maven Repository
- **deploy** - Ablegen des Artefaktes in das remote Maven Repository
### Maven Site Lifecycle
- **pre-site**
- **site**
- 