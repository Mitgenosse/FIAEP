# Mehrschichtenarchitektur

Eine Schichtenarchitektor (manchmal auch Schichtenmodell oder Schichtenmuster genannt) ist ein häufig angewandtes
Strukturierungsprinzuo für die Architektur eines Softwaresystems. Einzelne Aspekte eines Systems werden dabei konzeptionell in eine
Schicht (*tier* oder *layer* genannt) zugeordnet.

Die einzelnen Schichten sind zueinander so abhängig, dass Schichten einer höheren Ordnung nur schichten einer niedrigeren Ordnung verwenden dürfen.
Die Schichten bestehen je nach Art des Systems oder Detaillierungsgrads der Betrachtung z.B Funktionalitäten, Komponenten oder Klassen
sein.

### Vorteile

* Die Komplexität eines Systems wird vereinfacht, es entsteht eine leichter verständliche Anwendung.

### Zwei-Schichten-Architektur (*two tier architecture*)

Diese Art von Schicht besteht laut Namen aus zwei Schichten. Da nur höhere auf niedrigere Schichten zugreifen darf ist der Server
die niedrigere Schicht und der Client die höhere. Dies nennt man *Client-Server-Architektur*.

Die Rechenkapazität wird bei dieser Form häufig auf den Client-Rechner ausgelagert. 
Der Server bietet lediglich eine [Datenbankanwendung](Datenbankanwendung).

![Two Tier Architecture](https://github.com/Gurkenschreck/FIAEP/blob/master/content/resources/img/2-Tier.jpg)

### Drei-Schichten-Architektur (*three tier architecture*)

Bei einer dreischichtigen Architektur wird zwischen den Schichten der Zwei-Schichten-Architektur meist noch eine Logikschicht
zwischengeschaltet. Diese übernimmt die Datenverarbeitung.

Ein Drei-Schichten-Systems wie bei einem [Content-Management-System](CMS) besteht aus folgenden Schichten:

* Präsentationsschicht (*client tier*): Wird auch als Front-End bezeichnet und ist für die Representation 
der Daten, Benutzereingaben und die Benutzerschnittstellen verantwortlich.
* Logikschicht (*application-server tier*, Businessschicht, Middle Tier oder Enterprise Tier): Beinhaltet alle Verarbeitungsmechanismen.
Hier ist die Anwendungslogik abgebildet.
* Datenhaltungsschicht/Persistenzschicht (*data-server tier* oder *back end*): Enthält die Datenbank und ist für das Speichern und Laden von
Daten verantwortlich.

![Three Tier Architecture](https://github.com/Gurkenschreck/FIAEP/blob/master/content/resources/img/3-Tier.jpg)

### Resources
[Schichtenarchitektur Wikipedia](https://de.wikipedia.org/wiki/Schichtenarchitektur)