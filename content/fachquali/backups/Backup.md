# Backups

Ein Backup ist eine Sicherung von Daten (eines Rechners, Servers, etc.) um im Falle eines
Festplattenausfalls einen Datenverlust zu verhindern. Erstellte Sicherungen werden dann
im Falle eines Ausfalls dazu verwendet, den ursprünglichen Stand der Systeme wiederherzustellen.
Ein zweiter Nutzen besteht darin, dass man ältere gelöschte Dateien wiederherstellen kann. 

Es gibt also zwei Ziele:
1. Dateien im Falle eines Verlustes (gelöscht oder korrumpiert) wiederherstellen
2. Vor einiger Zeit gelöschte Dateien wiederherstellen

### Arten von Sicherungen

Es gibt verschiedene Arten Backups durchzuführen.

#### Komplett-/Vollsicherung

Bei einer Vollsicherung werden die zu sichernden Daten auf ein externes Speichermedium 
übertragen und als gesichert markiert. Die zu sichernden Daten können hier Laufwerke,
Partitionen, Verzeichnisse oder Dateien sein.  
Bei jeder weiteren Sicherung werden alle Daten noch einmal komplett gesichert.

Vorteile | Nachteile
--- | ---
Einfachste Möglichkeit | Sehr hoher Speicherbedarf

#### Differenzielle Sicherung

Bei der differenziellen Sicherung wird einmalig eine Vollsicherung durchgeführt. Wird nun ein
weiteres Mal gesichert, werden nur alle Abweichungen von der Vollsicherung gespeichert.
Dies hat den großen Vorteil, dass viel weniger Speicherplatz für mehrere
Sicherungen benötigt werden, als bei der Vollsicherung.
Die weiteren differenziellen Sicherungen sind unabhängig 
voneinander und können so einzeln gelöscht werden, ohne dass die Anderen beeinträchtigt werden.

Vorteile | Nachteile
--- | ---
Deutlich reduzierter Speicherbedarf gegenüber Vollsicherung | -
Zeitersparnis | -
Simpel handhabbar durch wenig Dateien | -

#### Inkrementelle Sicherung

Inkrementelle Sicherungen sichern die Veränderungen auf Basis der vorhergegangenen inkrementellen 
Sicherung. Dies bedeutet, dass die Sicherungen voneinander abhängig sind. Durch den sehr geringen
Speicherbedarf eignet sich das Verfahren in [Netzwerken](Netzwerk) oder der [Cloud](Cloud-Computing).
Durch die aufeinander aufbauenden Sichergungen kann das wiederherstellen von bestimmten Daten 
schwieriger werden, da dafür mehrere Sicherungen durchsucht werden müssen.

Vorteile | Nachteile
--- | ---
Benötigt am wenigsten Speicher | Erhöhte Komplexität
- | Sicherungen sind abhängig voneinander

### Revisionssicherheit

Für Unternehmen ergibt sich aus den gesetzlichen Vorschriften des [HGBs](Handelsgesetzbuch) eine
ordnungsgemäße, nachvollziehbare, revisionssichere Buchführung.

#### Was ist Revisionssicherheit?

Revisionssichere Archivierung bedeutet, dass die Daten/Informationen eines elektronischen
Systems jederzeit auffindbar, sicher, vollständig, ordnungsgemäß, unverändert, reproduzierbar,
verlustfrei gespeichert und verwaltet werden.

Wichtige Stichpunkte sind hierbei:
* Vollständigkeit
* Schutz vor Veränderung und Verfälschung
* Sicherung vor Verlust 
* Nutzung nur durch Berechtigte
* Dokumentation des Verfahrens 

### Umsetzung

#### Speichermedien

Medium | Max. Lebensdauer (Jahre) | Möglichke Beeinflussung der Lebensdauer
--- | --- | ---
CD | 30 | Wärme, Licht, Feuchtigkeit und Kratzer
DVD | 30 | Wärme, Licht, Feuchtigkeit und Kratzer
Blu-Ray Disk | 50 - 100 | Wärme, Licht, Feuchtigkeit und Kratzer
Solid-State-Disk | 10 | Beeinflusst durch Schreibzyklen
USB-Stick | 30 | Beeinflusst durch Schreibzyklen, mechanische Beanspruchung durch An-Abschließen
Externe Festplatte | 10 | Feuchtigkeit, Stöße, Magnetismus
Interne Festplatte | 5 - 10 | Wärme im Betrieb, Stöße

#### Aufbewahrungsorte

Die Speichermedien mit den Sicherungen sollten an unterschiedlichen Orten aufbewahrt werden.
So sollte ein mindestens Ort vor Feuer geschützt sein und ein anderer mindestens vor Wassereinbruch.
Die Sicherungen sollten an getrennten Orten aufbewahrt werden, möglichst nicht in der Firma.
Beispiele wären Bankschließfächer oder separate sichere Räume mit Tresor. 

### Resources
* [Was ist Revisionssicherheit?](http://www.ser.de/themen/was-ist-revisionssicherheit.html)
