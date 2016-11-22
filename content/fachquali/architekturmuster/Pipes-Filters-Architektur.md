# Pipes and Filters-Architektur

Das Pipes and Filters [Architekturmuster](Software-Architektur)
wird für Software-Systeme verwendet, das Datenströme verarbeitet. Jeder
Verarbeitungsschritt wird durch einen Filter realisiert und die
eigentlichen Daten werden durch Kanäle (engl. Pipes) geleitet.
Die Filter sind dabei sehr flexibel und lassen sich beliebig anordnen
und austauschen. Ein Beispiel für ein solches System ist der 
Kommandozeileninterpreter unter UNIX/LINUX. Der Aufruf eines Kommandos
liefert Daten, die dann über eine Pipe direkt an das nächste Kommando 
weitergeleitet werden.

### Resources
* [Pipes und Filter (Wikipedia)](https://de.wikipedia.org/wiki/Pipes_und_Filter)
