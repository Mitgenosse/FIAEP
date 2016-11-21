# Refactoring

Das Refactoring ist eine Methode um bestehenden Quellcode nachträglich zu
verbessern. Dabei wird der Quellcode unter den Gesichtspunkten von
Lesbarkeit, Wartbarkeit, Performance und Erweiterbarkeit analysiert und
verändert. Dabei dürfen keine Funktionalitäten der Software, ob beabsichtigt
oder unbeabsichtigt, verändert werden. Deshalb sind geeignete Vorsichts-
maßnahmen vor der Quellcodeveränderung sehr wichtig.

In der agilen Softwareentwicklung (z.B. Test-Driven Development) spielt
Refactoring eine besondere Rolle, da es dort oftmals ein ständiger Bestandteil
der Entwicklung ist.

### Ziele von Refactoring

Refactoring hat folgende Ziele:

1. Erhöhung der Lesbarkeit
2. Erhöhung der Wartbarkeit
3. Steigerung der Performance
4. Erhöhung der Erweiterbarkeit
5. Erhöhung der Testbarkeit
6. Redundanzenvermeidung

### Maßnahmen zur Fehlerprävention

Eine Maßnahme zur Fehlerprävention ist die Erstellung von Unit-Tests.
Diese Tests decken die Funktionalitäten eines Teilsystems ab. Sollte das
Refactoring nun unbeabsichtigt Teile des Systems verändern, kann dies 
schnell durch Unit-Tests getestet werden.

Quellcode sollte in kleineren Schritten refactored werden um Fehler zu
vermeiden.

Längerfristig sind Refactoring-Regeln sinnvoll, damit der Vorgang des
Refactorns langfristig die Codebasis einheitlich gestaltet wird.

### Resources
* [Test-Driven Development (Wikipedia)](https://en.wikipedia.org/wiki/Test-driven_development)