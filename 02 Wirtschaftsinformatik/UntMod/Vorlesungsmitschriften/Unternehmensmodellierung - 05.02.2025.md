# <font color = "orange">Unternehmensmodellierung - 05.02.2025</font>
### Ereignisbasiertes Gateway
Das Ereignisbasierte Gateway wartet auf ein bestimmtes Geschehen. Es wird dabei der [[Prozess]] geroutet auf den Pfad, dessen Ereignis zuerst eintritt.
Ereignisbasierte Gateways werden im Unternehmenskontext eher häufig verwendet, weil auf verschiedene Dinge gewartet wird.
Das Gateway hat ein Haus-Ähnliches Fünfeck in zwei Kreisen als Symbol.
>[!HINT] Die Zusammenführung geschieht über ein **exklusives Gateway**, da von mehreren Pfaden nur einer ankommen kann.

>[!WARNING] Das Ereignisbasierte Gateway entscheidet selbst, was geschieht und hat keine wirkliche Wahl; was geschieht ist vorgegeben und es gibt **keine aktive Entscheidung**.
## Symbole
### Brief
Eine Nachricht oder eine Zustellung
### Zeitereignis (Uhr)
Es wird gewartet, bis eine bestimmte Zeit abgelaufen ist.

## Ereignisse
Es sollte klar sein, dass Ereignisse in der Reihenfolge erwartet werden, wie sie modelliert wurden.
### Throwing Events
Throwing Events werden durch den Prozess selbst ausgelöst. Throwing Events werden immer schwarz dargestellt.
### Catching Events
Ereignisse, die außerhalb des Prozesses entstanden sind, werden im Prozess gefangen und dort verarbeitet. Catching Events werden immer hell als nicht ausgefülltes Symbol dargestellt.
### Startereignis
Startereignisse sind immer Catching Events
### Endereignis
Endereignisse sind immer Throwing Events.
### Terminierung
Es kann ein Event eintreten, nach dem der gesamte Prozess direkt abgebrochen werden soll. Dies wird durch die Terminierung ermöglicht.
## Typisierte Ereignisse
Eine Nachricht kann das Startereignisses eines Prozesses sein, aber auch ein Zwischenereignis oder ein Endereignis.
## Linientypen
### Sequenz
Eine Sequenz hat eine durchgezogene, schwarze Linie
### Nachricht
Eine Nachricht hat eine gestrichelte, schwarze Linie, die den Fluss einer Nachricht zeigt.