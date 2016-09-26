# Open Systems Interconnection model (OSI model)

...

### Die 7 Schichten

Das OSI Modell besteht aus 7 Schichten: 
1. Physical layer (Bitübertragung)
2. Data link layer (Sicherung)
3. Network layer (Vermittlung-/Paket)
4. Transport layer (Transport)
5. Session layer (Kommunikationssteuerung)
6. Presentation layer (Darstellung)
7. Application layer (Anwendungen)

Layer | Protocol data unit (PDU) | Funktion | Beispiele
--- | --- | --- | ---
7. Application | Daten | High-level APIs, einschließlich Ressourcensharing, Fernzugriff auf Daten | HTTP, HTTPS, NFS, FTP, Telnet, SMTP, SSH, LDAP
6. Presentation | Daten | Übersetzung von Daten zwischen Netzwerkservices und einer Applikation; Einschließlich character encoding, [Komprimierung](Komprimierung) und [Verschlüsselung](Kryptographie) | S/Mime, TLS
5. Session | Daten | Kommunikationssitzungen verwalten; durchgängger Informationsaustausch zwischen zwei Knoten | RPC, SCP, PAP
4. Transport | Segment (TCP) / Datagram (UDP) | Zuverlässige Übertragung von Segmenten zwischen Punkten im Netzwerk | TCP, UDP, NBF
3. Network | Paket | Verwaltung und Strukturierung eines Mehr-Knoten-Netzwerks, einschließlich Adressierung, Routing und Traffic Control | IPv4, IPv6, ICMP, IPsec, CLNP, DDP
2. Data link | Rahmen (Frame) | Zuverlässige Übertragung von Frames zwischen zwei Knoten, welche durch eine physische Schicht verbunden sind | IEEE 802.2, L2TP, LLDP, IEEE 802 Mac layers (Ethernet)
1. Physical | Bit | Übertragung und Empfang eines bit streams über ein physikalisches Medium | DSL, IEEE 802 physical layers (Ethernet), ISDN

### Resources
