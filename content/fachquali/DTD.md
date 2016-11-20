# Document type definition (DTD)

Eine document type definition gibt ein Schema vor, welches über die Struktur von Daten
Auskunft gibt. Sie wird in Verbindung mit [XML-Dateien](XML) verwendet und gibt an
wie die einzelnen XML ELemente aufgebaut sind und welche Informationen sie beinhalten können
(Datentyp, usw.).

### Beispiel DTD kunden.dtd

*Kommentar (unter der kommentierten Stelle)*

Dateiinhalt:  

```
<!ELEMENT adresse (name, strasse, wohnort, telefonnummern)>
                *Element mit beliebigem Element-Inhalt*
<!ELEMENT name (#PCDATA)>
<!ELEMENT strasse (#PCDATA)>
*Elementtyp mit einer beliebigen Zeichenkette als Inhalt*
<!ELEMENT wohnort (#PCDATA)>
<!ELEMENT telefonnummern (nummer)+> *Elementtyp mit beliebiger Wiederholung*
    <!ELEMENT nummer (#PCDATA)>
```

### Resources
* [Dokumenttypdefinition DTD (Wikipedia)](https://de.wikipedia.org/wiki/Dokumenttypdefinition)
* [DTD Tutorial (w3schools)](http://www.w3schools.com/XML/xml_dtd_intro.asp)
