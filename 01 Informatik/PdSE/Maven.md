# <font color = "orange">Maven</font>
>[!INFO] Definition
>Maven wurde von der Apache Software Foundation veröffentlicht. Das Tool ermöglicht das Builden und die Dokumentation von Projekten. Dafür nutzt Maven pom.xml-Files.

Maven sieht eine Standard-Verzeichnisstruktur vor. Diese unterscheidet sich nicht stark von der Standard-Struktur von IntelliJ.

## POM-Files
>[!HINT] **POM steht für *Project Object Model***.

Ein Maven-Projekt benötigt keinen Quellcode; ausschließlich eine pom.xml-Datei.
Eine POM-Datei beinhaltet:
- Dependencies
- Identifikatoren (Eindeutige IDs für das Projekt)
- Zugehörigkeit zu anderen POM-Files
- Enthaltene Module
- Eigenschaften (JRE)
- Build Einstellungen
- Weitere Projektinformationen
- Umgebungseinstellungen

Das Testen kann Teil des Buildings sein, sodass ein tatsächlich finaler Build ohne erfolgreiche Testphase gar nicht erst funktioniert.
### XML/Modell Einstellungen
In der Vorlesung wird fix `modelVersion 4.0.0` verwendet.
### Metadaten
- groupId: Eine GroupId sollte mit dem Pfad des Projektes auf dem Datenträger korrespondieren, muss aber nicht "C:\\" und so sein.
- artifactId: Der offizielle Name des Projektes
- version: die Version der Software, damit man identifizieren kann: groupId:artifactId
- type: .jar oder .war
- scope:
- optional: Erklärt, ob die Dependency zwangsweise zum Bauen des Projektes verfügbar sein muss, oder ob es auch ohne dieses Projekt funktioniert.
- dependencies: auch die Dependencies werden diesem Schema nach aufgeschrieben.
### Plugins
`plugins` beinhaltet Details zu Apache Plugins, in denen bspw das Maven-Jar-Plugin eingefügt werden kann. Dieses findet sich unter *MVN Repositories*.
### Reporting
Maven kann über Plugins nach dem Build anzeigen lassen, was für Vulnerabilities der Code beinhaltet. Dies läuft in einem eigenen Verzeichnis und lässt sich ebenfalls in der POM-File regeln.
Reports lassen sich bilden über beispielsweise das Plugin *maven-projekt-info-reports*