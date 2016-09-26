# Redundant Array of Independent Disks (RAID)

Ein Raid ist eine redundante Anordnung unabhängiger Festplatten.
Bei einem RAID-System handelt es sich um einen VErbund mehrerer Festplatten,
in dem Daten so gespeichert werden (mit Ausnahme von RAID 0), dass sie vor
Verlust geschützt sind.

RAID ersetzt kein Backup.

### RAID Varianten

Variante | Min. Festplatten | Beschreibung
--- | --- | ---
Einzeldisk | 1 | Diese Variante ist kein RAID-System. Sie ist der Standard.
JBOD | 2 | Mehrere Festplatten werden zu einem großen Laufwerk kombiniert.
RAID 0 | 2 | Es werden mehrere Festplatten für einem Geschwindigkeitsgewinn
miteinander verbunden. Hier werden Daten parallel auf verschiedene 
Festplatten verteilt. Ein NAS profitiert nicht von einem RAID 0, da
der Gewinn an Geschwindigkeit durch das Netzwerk gebremst wird.
Fällt eine Festplatte aus, sind alle Daten verloren.
RAID 1 | 2 | Bei diesem System steht die Datensicherheit im Vordergrund.
Alle Daten werden doppelt gespeichert. Bei Ausfall einer Platte sind die Daten
trotzdem gesichert. Dadurch wird zwar der insgesamt verfügbare Speicherplatz
eingeschränkt (halbiert), andererseits sind die Daten sicher. Ist eine
Platte ausgefallen, so ließt das [NAS](NAS) automatisch von der zweiten.
RAID 5 | 3 | Bei diesem System werden die Daten auch vor einem Ausfall geschützt.
Die Anzahl der nutbaren Festplatten beträgt n-1 da eine Platte für die Datensicherung
genutzt wird. Das System bietet mehr Geschwindigkeit als RAID 1. Fallen
zwei Platten gleichzeitig aus, sind die Daten verloren. Fällt eine Platte aus,
funktioniert zwar das RAID noch, es arbeitet jedoch langsamer.
RAID 5 + Spare | 4 | Siehe RAID 5. Hier ist eine Platte zusätzlich vorhanden,
welche als Reserve fungiert. Hier ist der gesamte Speicherplatz n-2 wobei
n die Anzahl der Platten ist.
RAID 6 | 4 | Hier werden zwei Platten zur Sicherung verwendet. Der Speicherplatz
ist der gleiche wie bei RAID 5 + Spare. RAID 6 ist durch die höhere Komplexität
langsamer. Dafür verkraftet RAID 6 auch zwei simultane Festplattenausfälle.



### Resources
* [PC-Welt - Was ist ein RAID-System?](http://www.pcwelt.de/ratgeber/Was-ist-ein-RAID-System-NAS-Server-445517.html)
