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