# Structured Query Language (SQL)

SQL steht für Structured Query Language (ungefähr strukturierte Abfragesprache) und ist eine
Sprache um Datenbanken zu manipulieren.

Relational Database Management System (RDBMS) ist die Basis für SQL und für alle modernen
[Datenbanksysteme](Datenbanksystem).

Daten werden in Tabellen innerhalb einer Datenbank gespeichert. Diese Tabellen besitzen
Spalten.

### Befehle und SQL-Kategorien

SQL-Kategorien
* DML (Data Manipulation Language)
* DDL (Data Definition Language)
* DCL (Data Control Language)
* Transaktionssteuerung

Kategorie | Befehle
--- | ---
DML | SELECT, INSERT, UPDATE, DELETE
DDL | CREATE, TRUNCATE, ALTER, DROP
DCL | GRANT, REVOKE
Transaktionssteuerung | ROLLBACK, COMMIT

### Wichtigste Befehle

Befehl | Funktion 
--- | ---
SELECT | Holt Daten aus einer Datenbank
UPDATE | Aktualisiert Daten in einer Datenbank
DELETE | Entfernt Daten aus einer Datenbank
INSERT INTO | Fügt neue Daten einer Datenbank hinzu
CREATE DATABASE | Erstellt eine neue Datenbank
ALTER DATABASE | Modifiziert eine Datenbank
CREATE TABLE | Erstellt eine neue Tabelle
DROP TABLE | Entfernt eine Tabelle
CREATE INDEX | Erstellt einen Index (Suchschlüssel)
DROP INDEX | Entfernt einen Index

### Abfragen / Syntax

#### SELECT, SELECT WHERE, SELECT DISTINCT

```
// Abfrage aller Spalten.
SELECT * from Customers;
// Abfrage von Name und Alter
SELECT NAME, AGE FROM Customers;
// Abfrage mit Bedingung (WHERE). Selektiere alle Spalten von Customers wessen Alter über 16 ist.
SELECT * FROM Customers WHERE AGE > 16;
// Abfrage mit DISTINCT, sodass doppelte Einträge in der Anzeige entfernt werden.
SELECT DISTINCT NAME FROM Customers;
```

/* TODO: mehr Abfragen einbauen */


Seletionsabfragen: SELECT, SELECT mit JOIN, SELECT mit Unterabfragen, SELECT mit Self-Join, SELECT mit Aggregatfunktionen

### Resources
* [SQL Tutorial (w3schools)](http://www.w3schools.com/sql/sql_intro.asp)
