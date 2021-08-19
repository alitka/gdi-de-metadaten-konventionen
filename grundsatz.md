[zurück zur Startseite](./)

# Grundsätzliche Konventionen für alle Metadaten
Die Konventionen in diesem Kapitel betreffen die Metadaten zu allen Ressourcen in der GDI-DE, unabhängig von der Art der Ressource im hierarchyLevel-Element (siehe 2.3).

## Multiplizität des identificationInfo-Elementes

|                        | verpflichtend | konditional | optional |
|:-----------------------|:--------------|:------------|:---------|
| GDI-DE                 |x              |             |          |
| zusätzlich für INSPIRE |               |             |          |

**```XPath:```** ```MD_Metadata/identificationInfo[1]```

Um die Einheitlichkeit und eindeutige Interpretierbarkeit der Metadaten in der GDI-DE zu fördern, gilt als Konvention für alle Metadaten in der GDI-DE:
Alle relevanten Informationen sind im ersten identificationInfo-Element anzugeben.
Gemäß [ISO 19115] kann das identificationInfo-Element innerhalb eines Metadatensatzes mehrfach verwendet werden. Im Rahmen von INSPIRE wird jedoch nur das erste identificationInfo-Element ausgewertet (siehe [INS TG MD], 2.3). Auch im Geoportal.de finden nur Informationen Berücksichtigung, die im ersten identificationInfo-Element angegeben sind.

[zurück zur Startseite](./)
