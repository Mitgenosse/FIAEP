# Extensible Markup Language (XML)

XML gehört zu der Gruppe der  Markup Languages, das heißt sie gibt die Struktur einer
Datei vor. Sie wurde entwickelt um Daten zu speichern und transportieren. Bei der 
Entwicklung wurde darauf geachtet, dass sie von Menschen und Maschinen lesbar ist.

### Data definition document (DTD)

Die Struktur einer XML-Datei kann durch ein [data definition document (DTD)](DTD) 
definiert werden.

### Beispiel XML kunden.xml

Das Beispiel DTD befindet sich im Artikel DTD.

*Kommentar (unter/bei der kommentierten stelle)*

Dateiinhalt:

```
<?xml version="1.0">
*Kennzeichnung der Datei als XML-Datei*
<!-- kundendaten -->
*Kommentar*
<!DOCTYPE kundendaten SYSTEM "kunden.dtd">
*Verweis auf die externe DTD-Datei*
<adresse>
    <name>Hans Kaiser</name>
    <strasse>Masurenallee 12</strasse>
    *Element mit Daten*
    <wohnort>20000 Hamburg</wohnort>
    <telefonnummern>
        <nummer>123456</nummer>
        <nummer>654321</nummer>
        *Wiederholdungselement*
        <nummer>111111</nummer>
    </telefonnummern>
</adresse
```

### Resources
* [XML Tutorial (w3schools)](http://www.w3schools.com/XML/default.asp)
