# <font color = "orange">TGDI 20.01.2025</font>
## Data Link Layer
Der Data Link Layer ist auf jedem Gerät inklusive, die irgendwie Knoten haben. 
Hosts sind Knoten im Netzwerk. Verbindungen zwischen direkt verbundenen Knoten sind Links.
Direktverbindungsnetze heißt, dass alle Knoten im Netzwerk erreichbar sind. Es lassen sich zudem alle Hosts über eine physikalische Adresse identifizieren. Eine Weiterleitung von Paketen von einem zu einem anderen Gerät wird allerdings noch nicht durchgeführt.

Eine Verbindung zwischen zwei Netzwerkknoten wird definiert durch:
- Übertragungsrate
- Übertragungsverzögerung
- Übertragungsrichtung [[Duplexmodi]]
- Mehrfachzugriffs (Multiplexing)

**Serialisierung**
Die Serialisierungszeit wird berechnet durch: $t_s = \frac{L}{r_{ij}}$. So rechnet man die Länge der Daten $L$ durch die Geschwindigkeit der Leitung $r$ zwischen den beiden Computern $i$ und $j$.

Die Übertragung dauert also eine Zeit, bis sie erreicht ist. Dann stellt sich die Frage, wie lang das ist. So wird nun die Dauer der Übertragung berechnet: $t_d=t_s+t_p$. $t_p$ steht dabei für die [[Ausbreitungsverzögerung]].

Es gibt verschiedene Topologien:
- Stern
	- In der Mitte ist der Switch und alle Geräte sind am Switch
- Vermaschung
- Vollvermaschung
	- Es gibt von jedem Gerät zu jedem Gerät eine Leitung, sodass es eine dedizierte Leitung für je zwei Geräte gibt
- Baum
	- Es gibt immer garantiert nur genau einen Weg, um von einem Gerät zu einem anderen zu kommen. 
	  >[!WARNING] Eine Vermaschung ist dieser Leitung vorzuziehen.
- BUS (Binary Unit System)
	- Es werden mehrere Teilnehmer direkt physisch an genau eine einzige Leitung gehängt. Es können keine zwei Teilnehmer miteinander reden, während andere miteinander reden. Gleichzeitig ist Routing nicht nötig. Allerdings können alle Teilnehmer alle Nachrichten mithören.

Auf der Sicherungsschicht wird der Medienzugriff geregelt.

## Multiplexen
- Zeitmultiplex:
	- Mehr oder weniger abwechselnd ( wie eine Ampel )
	- Deterministisch: Es wird im Voraus abgemacht, wer redet
	- Nicht deterministisch: Alle reden einfach mal und wenns ein Problem gibt wirds behoben
- Raummultiplex:
	- Durch räumliche Trennung können Frequenzen sich nicht überlappen und können so wiederverwendet werden
- Codemultiplex
	- Es werden unterschiedliche Alphabete je nach Empfänger verwendet
- ALOHA
	- Auf Hawaii entwickeltes Protokoll, nach dem es auch sein kann, dass es zu einer Kollosion kommt. Wenn ja, ist das ganze Datenpaket einfach wertlos.

## Bearbeitung Aufgaben
$L = 64\times 8 = 512$ Bit / Sekunde
Ausbreitungsverzögerung:
$v*c = \frac{2}{3} * 300.000 = 200.000$
*Gesucht: $d$* = 
