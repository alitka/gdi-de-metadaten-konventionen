# gdi-de-metadaten-konventionen
GDI-DE Architektur der Geodateninfrastruktur Deutschland - Konventionen zu Metadaten

<!-- tutorial for creating guthub-pages: https://academicpages.github.io/ -->

## Kapitel

[Einführung](./_pages/einfuehrung.html)

## Hinweise zum Dokument

Die Festlegungen in diesem Dokument sind für die Metadaten-Sprache „Deutsch“ getroffen, sofern  durch ISO oder INSPIRE keine anderen Forderungen bestehen.

Den einzelnen Festlegungen in diesem Dokument ist jeweils ein XPath-Ausdruck vorangestellt:

**```XPath:```**```MD_Metadata/```

Dieser adressiert bzw. beschreibt die Position des betreffenden Metadatenelementes im XML-Dokument. Die Kodierung des Elementes in XML wird jeweils wie folgt exemplarisch dargestellt:

**```Beispiel:```**```
<gmd:MD_Metadata>
...
</gmd:MD_Metadata>```

Die einzelnen Festlegungen des Dokumentes enthalten am Anfang jeweils folgende Tabelle:

| | verpflichtend | konditional | optional |
|:--|:--|:--|:--|
 GDI-DE | | | |
| zusätzlich für INSPIRE |  |  | |

Diese Tabelle gibt einen Überblick über die jeweilige Forderung der GDI-DE bzw. zusätzlich für INSPIRE. Dabei gelten folgende Festlegungen:

- „GDI-DE“ – generelle Konventionen für alle Metadaten, um eine Einheitlichkeit in den Metadaten der GDI-DE zu fördern und deren Interoperabilität zu gewährleisten. Diese Anforderungen können begründet sein
  - über [ISO 19115] und [ISO 19119] hinausgehende Festlegungen zwecks Einheitlichkeit;
  - durch die Verwendung der Metadaten für Open Data (siehe Kapitel 6);
  - durch Vorgaben seitens INSPIRE, für die eine Verallgemeinerung und Übertragung auf die gesamte GDI-DE als sinnvoll erachtet wurde.
- „zusätzlich für INSPIRE“ - Konventionen, die sich aus der RICHTLINIE 2007/2/EG DES EUROPÄISCHEN PARLAMENTS UND DES RATES vom 14. März 2007 zur Schaffung einer Geodateninfrastruktur in der Europäischen Gemeinschaft (INSPIRE), den INSPIRE
Implementing Rules oder den zugehörigen Technical Guidance-Dokumenten ergeben. Hierbei handelt es sich um Klarstellungen oder Präzisierungen der GDI-DE, um die Metadaten, die Ressourcen für INSPIRE beschreiben, einheitlich zu gestalten (z. B. in Fällen, in denen INSPIRE Freiräume zulässt). Grundsätzlich betrifft dies nur Metadaten, die Datensätze, -serien oder Netzdienste für INSPIRE beschreiben. Die Konventionen unter „GDI-DE“ (s.o.) sind dabei ebenfalls zu beachten und einzuhalten.
- _verpflichtend_ – generelle Verpflichtungen zur Erfüllung der Anforderungen seitens der GDI-DE bzw. für INSPIRE.
- _konditional_ - Verpflichtungen unter bestimmten Bedingungen, um die Anforderungen seitens der GDI-DE bzw. für INSPIRE zu erfüllen. Die jeweilige Konvention ist dann verpflichtend, wenn die benötigten Informationen vorliegen bzw. eine beschriebene Situation zutrifft.
- _optional_ - keine Verpflichtung zur Führung der jeweiligen Information. Für den Fall, dass diese Information aber erfasst werden soll, gelten die jeweils genannten Konventionen. 

Im Fließtext sind die Bezeichnungen von Metadatenelementen kursiv gesetzt, z. B.: _MD_Metadata_. Die Attributwerte sind in Anführungszeichen angegeben, z. B.: „Es gelten keine Bedingungen“.

Die dabei verwendeten Bezeichnungen von Metadatenelementen beziehen sich auf die Nomenklatur der Spezifikationen der [ISO 19115] und [ISO 19119] sowie der INSPIRE-Verordnung für Metadaten [INS VO MD].

Jede Festlegung in diesem Dokument endet mit einem Verweis auf die dazugehörige Testbeschreibung in Form einer Abstract Testsuite (ATS). Dort sind die jeweiligen Testschritte, welche in der GDI-DE Testsuite implementiert wurden, im Detail beschrieben:

**```ATS:```**```
https://ims.geoportal.de/git/tree/AK-Metadaten.git/version2.0.0/konventionen!ats```

Als Referenz werden unter https://ims.geoportal.de/git/tree/AK-Metadaten.git/version2.0.0/konventionen!beispiel_xml
Beispieldokumente bereitgestellt:
* dataset.xml (Daten-Metadatensatz)
* service.xml (Dienst-Metadatensatz)
* wms.xml (WMS-Capabilities-Dokument)
* opendata_dataset.xml (Daten-Metadatensatz)

In diesen Muster-Metadatensätzen sind die Konventionen, wie in diesem Dokument dargelegt, umgesetzt.

Dieses Dokument wird in einem stetigen Prozess fortgeschrieben und veröffentlicht. Je nach Veränderungen im Dokument werden die Versionsnummern wie folgt angepasst:

| Änderungen in der Versionsnummer |  Anlass bzw. Umfang der Änderung |
|:-- |:-- |
| 1. | Änderungen in den gesetzlichen Bestimmungen und damit grundsätzliche Änderungen im Dokument |
| 1.1 | Geringfügige Änderungen oder Ergänzungen in den Kapiteln, Ergänzung von neuen Kapiteln |
| 1.1.1 | Berichtigung von Schreibfehlern, Fehlerbehebung, redaktionelle Änderungen in den Kapiteln ohne fachliche Auswirkungen |
