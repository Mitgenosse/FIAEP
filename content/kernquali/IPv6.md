# Internet Protocol version 6 (IPv6)

IPv6 ist der Nachfolger von [IPv4](IPv4) und identifiziert einen Computer in einem [Netzwerk](Netzwerk). 
Eine IPv6 Adresse besteht aus 128 bits. Davon beschreiben die ersten 64 bits (von links nach rechts) das Routing Prefix und die letzten
64 bits die Host-ID im Netzwerk.
/* TODO: Route Prefix und Interface ID fixen */

Die gesamte Adresse besteht aus 16 * 4 bit Blöcken welche in base16 (Hexadezimal) codiert sind (Darstellung durch Buchstaben von [0-9A-F].

Die Anzahl der Kombinationsmöglichkeiten bei 128 bits beträgt 2^128 = 3,4*10^38 (gerundet)

### Darstellung (und Kürzung)

Es gibt 3 Regeln um eine IPv6 Adresse darzustellen.

Regel 0, Standard:
Alle 16 bits (4 hexadezimale Zeichen) werden durch einen : getrennt. Diese markieren einen Block.

Regel 1:
Führende Nullen können entfernt werden.

Beispiel:
```
2001:0db8:01F0:3100:FFAD:0002:0001
2001:db8:1F0:3100:FFAD:2:1
```

Regel 2:
Bestehen zwei oder mehr Blöcke aus Nullen so können diese komplett weggelassen werden.

Beispiel:
```
2001:0db8:0000:0000:0000:0000:0000:0001
2001:0db8::0001 (Blöcke entfernt)
2001:db8::1 (Führende Nullen entfernt)
```

### Vorteile

IPv6 hat gegenüber seinem Vorgänger IPv4 einige Vorteile.

* **Adressraum**: Durch die 128 bits hat IPv6 einen viel größeren Adressraum gegenüber IPv4 mit 32 bits.
* **Simplifizierter Header**: Der Header von IPv6 wurde vereinfacht, indem unbenötigte Informationen ans Ende des Headers verschoben wurden. Der Header ist nur zwei mal so groß als bei IPv4.
* **Eindeutige Adressen**: Durch die hohe Anzahl der verfügbaren Adressen kann jedes Gerät im Netzwerk eine eigene Adresse bekommen. Dies ermöglicht das versenden von Paketen ohne NAT oä. Einschränkungen können durch Firewall oder Unternehmensrichtlinien durchgeführt werden.
* **Auto Konfiguration**: IPv6 unterstützt die stateful and
* **Schnellere Weiterleitung/Routen**: ...
* **Anycast**: ...
* **Mobilität**: IPv6 wurde unter Betrachtung der Mobilität entwickelt. Darum ist es möglich den geographischen Standort eines Hosts zu wechseln, ohne dass sich die IPv6 Adresse ändert.
* **Erweiterbarkeit**: ...
* **Smooth Transition**: ...
* **Enhanced Priority support**: ... 

/* TODO: Auto Konfiguration besser beschreiben */

### Reservierte Adressen

Adressenprefix | Beschreibung
--- | ---
fe80:: | Dieser Prefix beschreibt eine Link-Local Adresse.
2001:db8:: | Dieser Prefix wird in Dokumentationen und Beschreibungen verwendet. Sie ist keine routbare Adresse.

### Adressierungsmodus (Unicast, Multicast, Anycast)

Der Adressierungsmodus beschreibt wie Rechner die Empfänger eines Pakets adressieren.

Art | Beschreibung
--- | ---
Unicast | Bei Unicast wird ein Paket an einen bestimmten Rechner übermittelt.
Multicast | Mit Multicast wird ein Paket an jeden Rechner einer Gruppe von Rechnern versendet.
Anycast | Bei Anycast wird ein Paket and den nächsten Rechner einer Gruppe von Rechnern versendet.

### Subnetting

### Resources 
