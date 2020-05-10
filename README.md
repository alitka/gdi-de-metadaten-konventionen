# gdi-de-metadaten-konventionen
GDI-DE Architektur der Geodateninfrastruktur Deutschland - Konventionen zu Metadaten

<!-- tutorial for creating guthub-pages: https://academicpages.github.io/ -->

# Einführung
## Die Architektur der Geodateninfrastruktur Deutschland
Um ein reibungsloses Zusammenwirken der nationalen technischen Komponenten der GDI-DE zu ermöglichen, sind organisatorische und technische Rahmenvorgaben erforderlich, die zusammenfassend als Architekturkonzept der GDI-DE bezeichnet werden. 

Zur leichteren Handhabung ist das Architekturkonzept der GDI-DE aus einzelnen Dokumenten in drei verschiedenen Kategorien (grundsätzliche Festlegungen, spezielle technische Festlegungen und Empfehlungen) aufgebaut:

![img_aufbau](https://raw.githubusercontent.com/alitka/gdi-de-metadaten-konventionen/master/images/img_aufbau.png)

Grundsätzliche Festlegungen werden durch Beschluss des LG GDI-DE in folgenden Dokumenten getroffen:

* Das Dokument .[„Architektur der GDI-DE - Ziele und Grundlagen“](https://www.gdi-de.org/SharedDocs/Downloads/DE/GDI-DE/Architektur_Ziele_und_Grundlagen_v3_1_2.pdf) erläutert die strategischen Ziele, fachliche und technische Grundsätze sowie die rechtlichen und organisatorischen Rahmenbedingungen der GDI-DE.
* Das Dokument .[„Architektur der GDI-DE - Technik“](https://www.gdi-de.org/SharedDocs/Downloads/DE/GDI-DE/Dokumente/AK_Architektur_GDI-DE_Technik_V_3_4_1.pdf) beschreibt die verschiedenen Architektur- komponenten und referenziert hierfür relevante Normen, Standards und Spezifikationen.
* Das Dokument .[„Architektur der GDI-DE - Maßnahmenplan“](https://www.gdi-de.org/SharedDocs/Downloads/DE/GDI-DE/Dokumente/AK_Architektur_GDI-DE_Ma%C3%9Fnahmenplan_V3_4_0.pdf) zeigt die für die künftige Entwicklung der GDI-DE erforderlichen Schritte auf

Spezielle technische Festlegungen, vor allem in Bezug auf Technik und Betrieb von Komponenten der GDI-DE, werden durch Beschluss des LG GDI-DE in folgenden Dokumenten getroffen:

* Profile der GDI-DE zu internationalen oder nationalen Normen und 
* Konventionen, die über eine Norm oder Spezifikation hinausgehen.

Darüber hinausgehende Informationen werden als Handlungsempfehlungen von Arbeitskreisen weiter konkretisiert.

## Konventionen zu Metadaten

Im vorliegenden Dokument werden Konventionen zu Metadaten sowie deren Bereitstellung erläutert und zusammengefasst. Diese Konventionen werden im Arbeitskreis (AK) Metadaten erarbeitet. Ältere Vorgängerversionen gehen auch auf Arbeiten der Projektgruppe Geodatenkatalog.de und einen Metadaten-Workshop mit Ansprechpartnern der GDI-DE aus Bund und Ländern zurück. Weitere Hinweise, welche sich auf die Inhalte von Metadaten beziehen, finden sich in eigenen Handlungsempfehlungen, z. B. der Länder-GDIs 1 , wieder.

In Geodateninfrastrukturen gibt es grundsätzlich zwei unterschiedliche Typen von Metadatendokumenten:

* Typ1: Capabilities-Dokumente, mit welchen Dienste-Schnittstellen ihre Eigenschaften beschreiben.
* Typ2: Metadaten nach ISO 19115/19119, welche in Katalogen erfasst und bereitgestellt werden.

Das vorliegende Dokument befasst sich überwiegend mit Konventionen zu Typ 2. Typ 1 wird in den Konventionsdokumenten bzw. Handlungsempfehlungen des AK Geodienste behandelt.

Grundsätzlich sollen in der GDI-DE sowohl die Anforderungen aus der INSPIRE-Richtlinie (sofern relevant) als auch die ISO-Festlegungen [ISO 19115, ISO 19119, ISO 19139] erfüllt werden. Alle Vorgaben der ISO (Belegungspflichten bzw. -bedingungen, Werteumfänge etc.) gelten somit auch für die GDI-DE. Das bedeutet, dass es weitere, zwingend zu belegende Metadatenelemente geben kann, die benötigt werden, um einen ISO- und/oder INSPIRE-konformen Metadatensatz zu bilden, auch wenn das vorliegende Dokument keine Konvention dazu aufführt.

Ergänzend bzw. vertiefend werden in diesem Dokument konkrete Konventionen für einzelne Metadatenelemente in der GDI-DE beschrieben. Die Festlegungen im vorliegenden Dokument betreffen Metadatenelemente, für die Regelungsbedarf in der GDI-DE gesehen wird, der über die grundsätzlichen Regelungen der ISO hinausgehen kann oder aus verpflichtenden oder bedingten
Angaben für INSPIRE resultiert.

Außerdem trifft dieses Dokument keine Festlegungen zur inhaltlichen Strukturierung von Freitext-Elementen wie z. B. Titel und Kurzbeschreibung. Etwaige Regelungen für eine einheitliche Vergabe von Titeln, Kurzbeschreibungen etc. und die Festlegung von Benennungsmustern liegen im Ermessen der einzelnen Fachnetzwerke und sind durch diese in eigenen Leitfäden zu treffen.

Bzgl. der Vorgaben seitens INSPIRE wird an dieser Stelle explizit darauf hingewiesen, dass zzt. für die GDI-DE keine Betrachtung der sog. „aufrufbaren Geodatendienste“, die keine INSPIRE-Netzdienste sind, erfolgt. Aus der INSPIRE Technical Guidance zu Metadaten V2.0.1 wurden daher nur die Belange für Metadaten zu Datensätzen und -serien sowie zu Netzdiensten berücksichtigt. Die Vorgaben für aufrufbare Geodatendienste gelten seitens INSPIRE davon unbenommen; eine Präzisierung durch die GDI-DE bleibt jedoch zzt. aus, weil momentan keine Anwendungsfälle existieren. Bei Bedarf wird dies zu einem späteren Zeitpunkt im Rahmen der Fortschreibung dieses Dokumentes ergänzt.

## Die Topologie der Metadatenkataloge

In der GDI-DE existieren eine Vielzahl verteilter, eigenständiger Metadatenkataloge, deren Inhalte im zentralen Geodatenkatalog.de zusammengeführt werden. Eine ähnliche Aggregation geschieht auch in anderen Knoten. Beispielsweise laufen in den Katalogen der Bundesländer die Metadaten aus verschiedenen Bereichen und Ebenen der Verwaltung zusammen. Abbildung 2 verdeutlicht diesen Zusammenhang.

Eine Beschreibung der zentralen Komponente „Geodatenkatalog.de“ der GDI-DE erfolgt in diesem Dokument nicht, sondern ist im Dokument „Architektur der GDI-DE – Technik“ zu finden. Dort werden auch die Voraussetzungen für die Einbindung einer dezentralen Katalogschnittstelle in die GDI-DE beschrieben.

Durch die Topologie der Metadatenkataloge ist es notwendig, dass Änderungen eines Katalogs überall dort nachvollzogen werden, wo dessen Bestand übernommen wird. Wird also ein Metadatensatz in einem Katalog gelöscht, so wird er auch in allen anderen Katalogen entfernt, welche diesen Katalog harvesten, da der fileIdentifier des Metadatensatzes und damit der Metadatensatz
selbst nicht mehr auffindbar ist. Übernommen werden zugleich alle „neuen“ Metadaten mit einem bisher nicht vorhandenen fileIdentifier und alle geänderten Metadaten, deren fileIdentifier bereits bekannt sind, die jedoch einen aktualisierten Zeitstempel tragen.

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
