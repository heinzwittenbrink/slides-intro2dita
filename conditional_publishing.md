---
title: Bedingtes Publizieren mit DITA
author: Heinz Wittenbrink
date: 2018-03-17
---

# Ziel heute: 

Praktische Erfahrung mit grundlegenden DITA-Dokumenttypen und ihrem Zusammenspiel

# Was wissen wir über DITA?

- Topicbasiert
- Vielfältiger Output
- Vererbung und Spezialisierung
- Conditional Publishing

# Beispiel heute:

[Using Framemaker 2015 and ditaval to publish maps for specific audience/Product/Platform -YouTube](https://www.youtube.com/watch?v=zHht9HHw9u8)

# Topics

# Concepts

# Tasks

# References

# Maps

# ditaval

# Bedingtes Verarbeiten

-  `ditaval`-Dateien enthalten Profile für die bedingte Verarbeitung
- Filtern: bestimmen, welche Inhalte in eine Publikation aufgenommen werden
- Flaggen/kennzeichnen: Bestimmte Elemente im Output hervorheben
- `ditaval`-Dateien arbeiten mit Attributen der Inhalte

# .ditaval file sample 
```xml
<source lang="xml">
<?xml version="1.0" encoding="UTF-8"?>
<val>
  <prop att="audience" val="foo" action="include" />
  <prop att="audience" val="bar" action="exclude" />
</val>
</source>
```

# Attribute 

- `audience`: bestimmt die Zielgruppe
- `platform`: bestimmt die Software oder Harware-Plattform
- `importance`: bestimmt die Wichtigkeit einer Information
- `product`: bestimmt Produkt oder Produktversion

(Quelle: [data2type GmbH: DITA | Topics von Inhalten erstellen](https://www.data2type.de/xml-xslt-xslfo/dita/bedingte-verarbeitung/topics-fuer-das-filtern-und-ke/))

# Weitere Attribute

- `rev`: bestimmt Änderungszustände
- `otherprops`: für Sitituationen, in denen die vorhandenen Attribute nicht ausreichen. 
- `status`: bestimmt den Status eines Elements
- `props`: generisches Attribut für die Spezialisierung

(Quelle: [data2type GmbH: DITA | Topics von Inhalten erstellen](https://www.data2type.de/xml-xslt-xslfo/dita/bedingte-verarbeitung/topics-fuer-das-filtern-und-ke/))


# content reference als Alternative

- Bedingte Verarbeitung kann zu übergroßer Komplexität führen
- content references (`conref`) wiederholen Inhalte in unterschiedlichen Kontexten 

Siehe: @bellamy2012

# Reflexion über XML

- Semistrukturierte Daten
- Content-Modellierung
- Strukturiertes Authoring

# Aufgabe

- Kommentierung von Beispielen für Concept, Task, Reference, Map

- Quelle für Beispiele: [GitHub - gnostyx/dita-demo-content-collection: DITA Demonstration Content Collection](https://github.com/gnostyx/dita-demo-content-collection)

- Online Session: 12. April, 19:30, URL: https://zoom.us/j/894321493

# Literatur: 
