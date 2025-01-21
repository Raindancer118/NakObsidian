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

### XML/Modell Einstellungen
In der Vorlesung wird fix `modelVersion 4.0.0` verwendet.

### Metadaten
- groupId: 