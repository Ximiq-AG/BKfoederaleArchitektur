# Core Public Servce Vocabulary Applications Profile (CPSV-AP)

## Öffentliche Dienstleistung

Eine öffentliche Dienstleistung ist eine obligatorische oder freiwillige Reihe von Aktivitäten, die von oder im Namen einer öffentlichen Organisation erbracht werden oder erbracht werden können, öffentlich finanziert werden und sich aus der rechtlichen und ordnungspolitischen Rahmenordnungöffentlichen Ordnung   ergeben. Die Dienstleistungen können für einer Einzelperson, einem Unternehmen, einer anderen öffentlichen Behörde oder einer Gruppe von diesen von Nutzen sein. Eine öffentliche Dienstleistung besteht unabhängig davon, ob sie in Anspruch genommen wird oder nicht, und der Begriff "Nutzen" kann im Sinne der Erfüllung einer Verpflichtung verwendet werden.

|Klassenname|Obligatorisch/Optional|URI|
|---|---|---|
|Öffentliche Dienstleistung|Obligatorisch |

Die folgenden Unterabschnittenachfolgenden Kapitel definieren die Attribute der Klasse Öffentliche Dienstleistung.

### Identifikator

Dieses Attribut stellt einen formell ausgestellten Identifikator für die öffentliche Dienstleistung dar.

|Attribut|URI |Range|Kardinalität |
|---|---|---|---|
|identifikator|dct:identifier |Text|1..1|

### Name

Dieses Attribut stellt den offiziellen Namen der öffentlichen Dienstleistung dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
name |dct:title |Text |1..1

### Beschrieb

Dieses Attribut stellt einen Freitextbeschrieb der öffentlichen Dienstleistung dar. Der Text sollte mit dem Beschrieb der öffentlichen Dienstleistung im Behördenleistungsverzeichnis auf der Interoperabilitätsplattform des Bundes übereinstimmen.   Öffentliche Organisationen werden ermutigt, im Beschrieb ein angemessenes Mass an Details aufzunehmen.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
beschrieb |dct:description |Text |1..1

### Schlüsselwort

Dieses Attribut stellt ein einen Begriff oder einen Satz  dar, der die öffentliche Dienstleistung beschreibt.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
schlüsselwort |dcat:keyword |Text |0..n

### Sektor

Dieses Attribut steht für die Branche oder den Sektor, auf den sich eine öffentliche Dienstleistung bezieht bzw. für den sie bestimmt ist. Zum Beispiel: Umwelt, Sicherheit, Wohnen. Beachten Sie, dass eine einzelne öffentliche Dienstleistung mehrere Sektoren betreffen kann. Die möglichen Werte für dieses Attribut werden als kontrolliertes Vokabular   bereitgestellt.  

Attribut |URI |Range |Kardinalität
|---|---|---|---|
sektor |cv:sector |Konzept |0..n

### Themenbereich

Dieses Attribut stellt den thematischen Bereich einer öffentlichen Dienstleistung dar, wie er in einem kontrollierten Vokabular beschrieben wird, z. B. Sozialschutz, Gesundheit, Freizeit, Kultur und Religion, Familie, Reisen, Wirtschaft, Steuern, Personal, Umwelt...

Attribut |URI |Range |Kardinalität
|---|---|---|---|
themenbereich |cv:thematicArea |Konzept |0..n

### Art

Dieses Attribut stellt die Art einer öffentlichen Dienstleistung dar, wie sie in einem kontrollierten Vokabular beschrieben wird. Bei der Angabe der Art beziehen wir uns auf die Funktionen der Regierung, um den Zweck einer Regierungstätigkeit anzugeben, für den die öffentliche Dienstleistung bestimmt ist.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
art |dct:type |Konzept |0..n

### Sprache

Dieses Attribut steht für die Sprache(n), in der/denen die öffentliche Dienstleistung verfügbar ist. Dabei kann es sich um eine Sprache oder um mehrere Sprachen handeln. Die möglichen Werte für Dieses Attribut werden in einem kontrollierten Vokabular beschrieben .
ISO 639-1

Attribut |URI |Range |Kardinalität
|---|---|---|---|
sprache |dct:language |dct:LinguisticSystem |0..n

### Status

Dieses Attribut gibt an, ob ein öffentlicher Dienst aktiv, inaktiv, in der Entwicklung ect. ist. Die möglichen Werte für dieses Attribut werden in einem kontrollierten Vokabular beschrieben.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
status |adms:status |Konzept |0..1

### Ist Gruppiert Nach

Dieses Attribut verknüpft eine öffentliche Dienstleistung mit der Klasse Ereignis. Ein bestimmtes Ereignis kann mit mehreren öffentlichen Dienstleistungen, und eine öffentliche Dienstleistung mit mehreren verschiedenen Ereignissen verbunden sein.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
istGruppiertNach |cv:isGroupedBy |Ereignis |0..n

### Bedingt 

Eine öffentliche Dienstleistung kann das Ergebnis einer oder mehrerer anderer öffentlicher Dienstleistungen erfordern oder in irgendeiner Weise nutzen. In diesem Fall muss für die Ausführung der öffentlichen Dienstleistung eine andere öffentliche Dienstleistung vorher ausgeführt werden. Die Art der Bedingung wird in der zugehörigen Regel beschrieben.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
bedingt |dct:requires |Öffentliche Dienstleistung |0..n

### Ist verbunden mit

Dieses Attribut stellt eine öffentliche Dienstleistung dar, die mit einer bestimmten Instanz der Klasse öffentliche Dienstleistung verbunden ist.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
istVerbundenMit |dct:relation |Öffentliche Dienstleistung |0..n

### Hat Bedingung

Verknüpft eine öffentliche Dienstleistung mit einer Klasse, die die Bedingungen für den Bedarf oder die Inanspruchnahme der öffentlichen Dienstleistung beschreibt, z. B. Wohnsitz an einem bestimmten Ort, ein bestimmtes Alter usw.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
hatBedingung |cv:hasCriterion |Bedingung |0..n

### Ist zuständig

Dieses Attribut verknüpft eine öffentliche Dienstleistung mit einer öffentlichen Organisation, die für die Erbringung der öffentlichen Dienstleistung verantwortlich ist. Dabei ist es unerheblich, ob die betreffende öffentliche Organisation die öffentliche Dienstleistung direkt erbringt oder auslagert. Die öffentliche Organisation, die für die öffentliche Dienstleistung zuständig ist, ist diejenige, die letztendlich für die Verwaltung und Erbringung der öffentlichen Dienstleistung verantwortlich ist.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
 istZuständig |cv:hasCompetentAuthority |Öffentliche Organisation |1..1

### Hat Beteiligung

Das CPSV-AP definiert die Rolle der öffentlichen Organisation, aber dieses einfache Modell kann bei Bedarf durch das Attribut «Hat Beteiligung» erweitert werden, die auf die Klasse Beteiligung verweist.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
hatBeteiligung |cv:hasParticipation |Beteiligung |0..n

### Hat Input

Das Attribut «Hat Input» verknüpft eine öffentliche Dienstleistung mit einer oder mehreren Instanzen der Klasse «Nachweis». Eine öffentliche Dienstleistung kann das Vorhandensein eines bestimmten Nachweises erfordern, um erbracht zu werden. Wenn der Nachweis, die für den Bezug einer öffentlichen Dienstleistung über einen bestimmten Kanal erforderlich ist, dann sollte «Hat Input» auf der Ebene des Kanals liegen.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
hatInput |cpsv:hasInput |Nachweis |0..n

### Hat Rechtsgrundlage

Das Attribut «Hat Rechtsgrundlage» verknüpft eine öffentliche Dienstleistung mit einer Rechtsgrundlage. Sie gibt die Rechtsgrundlage an, auf die sich die öffentliche Dienstleistung bezieht oder die sie ausübt.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
hatRechtsgrundlage |cv:hasLegalResouce |Rechtsgrundlage |0..n

### Erzeugt

Das Attribut «erzeugt» verknüpft eine öffentliche Dienstleistung mit einer oder mehreren Instanzen der Klasse «Ergebnis», die das tatsächliche Ergebnis der Ausführung einer bestimmten öffentlichen Dienstleistung beschreibt. Ergebnisse können beliebige Ressourcen sein, z. B. ein Dokument, ein Artefakt oder Ähnliches, das als Ergebnis der Ausführung der öffentlichen Dienstleitung erzeugt wird.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
erzeugt |cpsv:produces |Ergebnis |0..n

### Folgt

Das Attribut «folgt» verknüpft eine öffentliche Dienstleistung mit der/den Regel(n), nach der/denen sie arbeitet. Die Definition der Klasse "Regel" ist sehr weit gefasst. In einem typischen Fall wird die zuständige öffentliche Organisation, die die öffentliche Dienstleistung erbringt, auch die Regeln zur Umsetzung ihrer eigenen Politik definieren. 

Attribut |URI |Range |Kardinalität
|---|---|---|---|
folgt |cpsv:follows |Regel |0..n

### RäumlicheZuordnung

Es kann sein, dass eine öffentliche Dienstleistung nur in einem bestimmten Gebiet verfügbar ist, typischerweise in dem von einer bestimmten öffentlichen Organisation abgedeckten Gebiet. Eine übliche Verwendung dieses Attributs besteht darin, die administrative(n) Gebietseinheit(en) - in der Regel der Bund, ein Kanton oder eine Gemeinde - zu definieren, in der eine öffentliche Dienstleistung verfügbar ist.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
räumlicheZuordnung |dct:spatial |Location |0..n

### Hat Kontaktstelle

Der Wert des Attributs «hat Kontaktstelle», die Kontaktinformationen selbst, sollte mit schema:ContactPoint angegeben werden. Beachten Sie, dass die Kontaktinformationen für die öffentliche Dienstleistung relevant sein sollten, und daher nicht unbedingt mit den Kontaktinformationen der zuständigen öffentlichen Organisation oder einer beteiligten Organisation übereinstimmt.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
hatKontaktstelle |cv:hasContactPoint |Kontaktstelle |0..n

### Hat Kanal

Dieses Attribut verknüpft die öffentliche Dienstleistung mit einem beliebigen Kanal, über den ein Agent die öffentliche Dienstleistung anbietet, nutzt oder anderweitig mit ihr interagiert, wie z. B. ein Online-Dienst, eine Telefonnummer oder ein Schalter.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
hatKanal |cv:hasChannel |Kanal |0..n

### Bearbeitungszeit

Der Wert dieses Attributs ist die (geschätzte) Zeit, die für die Ausführung einer öffentlichen Dienstleistung benötigt wird. Die tatsächliche Information wird unter Verwendung der ISO8601-Syntax für Zeitdauern angegeben. Im Folgenden werden einige Beispiele angeführt:

Durations begin with an uppercase P followed by the number and the relevant designator, formally: P[n]Y[n]M[n]DT[n]H[n]M[n]S, where Y is for years, M for months etc. Note that days and times are separated by an uppercase T which also disambiguates M as meaning month (P2M means 2 months) or minute (PT2M means 2 minutes). Durations may also be defined as a number of weeks so P4W means 4 weeks. A full explanation is provided in the Wikipedia page that references the official ISO standard.

This approach is consistent with both schema.org and the W3C OWL Time Ontology.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
bearbeitungszeit |cv:processingTime |Duration |0..1

### Hat Gebühr

Das Attribut «Hat Gebühr» verknüpft eine öffentliche Dienstleistung mit einer oder mehreren Instanzen der Klasse «Gebühr». Sie gibt die Kosten an, die mit der Ausführung einer öffentlichen Dienstleistung für eine natürliche oder juristische Person verbunden sind. Wenn die Kosten je nach Kanal, über den auf die öffentliche Dienstleistung zugegriffen wird, variieren, können sie über die Beziehung «wenn zugegriffen über» mit dem Kanal verknüpft werden.

|Attribut|URI|Range|Kardinalität|
|---|---|---|---|
|hasGebühr|cv:hasCost|Gebühr|0..n|

### Ist beschrieben in

Das Attribut «Ist beschrieben in» verknüpft eine öffentliche Dienstleistung mit dem/den Datensammlung/en, in dem sie beschrieben wird.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
istBeschriebenIn |cv:isDescribedAt |Datensammlung |0..n

### Ist klassifiziert durch

Das Attribut «Ist klassifiziert durch» ermöglicht die Klassifizierung von öffentlichen Dienstleistungen nach einem beliebigen Konzept, das nicht bereits in der CPSV-AP vorgesehen und explizit definiert ist. Es handelt sich um eine generisches Attribut, das weiter spezialisiert werden kann, um die Klassifizierung explizit zu machen, z. B. für die Klassifizierung von öffentlichen Dienstleistungen nach Digitalisierungsgrad, Art des Publikums ...

Attribut |URI |Range |Kardinalität
|---|---|---|---|
istKlassifiziertDurch |cv:isClassifiedBy |Konzept |0..n

## Ereignis

Diese Klasse repräsentiert ein beliebiges Ereignis, das eine öffentliche Dienstleistung auslöst, nutzt oder in irgendeiner Weise mit ihr verbunden ist. Es wird nicht erwartet, dass die Klasse direkt verwendet wird, vielmehr sollte eine ihrer Unterklassen verwendet werden. Die Eigenschaften der Klasse werden an diese Unterklassen vererbt. Die Klasse "Ereignis" wird entweder als Auslöser für eine einzelne öffentliche Dienstleistung verwendet, z. B. die Diagnose einer Krankheit im Zusammenhang mit einem Antrag auf Leistungen der Invalidenversicherung, oder für eine Gruppe von öffentlichen Dienstleistungen, z. B. alle Dienstleistungen im Zusammenhang mit der Gründung eines neuen Unternehmens.

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Ereignis |Optional |

Die folgenden Unterabschnitte definieren die Attribute der Klasse Ereignis.

### Identifikator

Dieses Attribut stellt einen Identifikator für das Ereignis dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
identifikator |dct:identifier |Text |1..1

### Name

Dieses Attribut stellt den Namen oder Titel des Ereignisses dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
name |dct:title |Text |1..1

### Beschrieb

Dieses Attribut stellt einen Freitextbeschrieb des Ereignisses dar. Der Beschrieb sollte der Text sein, den ein Unternehmen oder ein Bürger für dieses spezifische Ereignis sieht, wenn er nach relevanten öffentlichen Dienstleistungen sucht. Öffentliche Organisationen werden daher aufgefordert, eine angemessene Detailtiefe in den Beschrieb aufzunehmen.  

Attribut |URI |Range |Kardinalität
|---|---|---|---|
beschrieb |dct:description |Text |0..1

### Art

Das Attribut "Art" verknüpft ein Ereignis mit einem kontrollierten Vokabular von Ereignistypen  , und es ist die Art dieser kontrollierten Vokabulare, die den Hauptunterschied zwischen einem Geschäftsereignis, wie z. B. der Gründung des Unternehmens, und einem Lebensereignis, wie z. B. der Geburt eines Kindes, darstellt.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
art |dct:type |Konzept |0..n

### Verbundene Dienstleistung

Dieses Attribut verknüpft ein Ereignis direkt mit einer öffentlichen Dienstleistung, die mit ihm in Verbindung steht.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
verbundeneDienstleistung |dct:relation |Öffentliche Dienstleistung |0..n

## Geschäftsereignis

Ein Geschäftsereignis ist eine bestimmte Situation oder ein Ereignis eines Unternehmens, welches ein oder mehrere Bedürfnisse oder Verpflichtungen dieses Unternehmens entstehen lässt. Ein Geschäftsereignis erfordert die Bereitstellung und Inanspruchnahme einer oder mehreren öffentlichen Dienstleistungen, damit die damit verbundenen geschäftlichen Bedürfnisse oder Verpflichtungen erfüllt werden können. Geschäftsereignisse werden im Kontext eines bestimmten Landes definiert. Mit anderen Worten, ein Geschäftsereignis fasst die öffentlichen Dienstleistungen zusammen, die wegen des Ereignisses in Anspruch genommen werden müssen.

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Geschäftsereignis |Optional |

## Lebensereignis

Die Klasse "Lebensereignis" steht für ein wichtiges Ereignis oder Situation im Leben eines Bürgers/einer Bürgerin, in denen öffentliche Dienstleistungen erforderlich sind. Eine Person wird mit einer beliebigen Anzahl von "Ereignissen" konfrontiert. Lebensereignisse sind nur personenbezogene Ereignisse, mit denen eine öffentliche Dienstleistung verbunden ist. So ist beispielsweise die Verlobung eines Paares kein Lebensereignis, die Heirat aber schon, da sie öffentliche Dienstleistungen (Bsp. Registrierung des neuen Zivilstandes beim Zivilstandsamt) zur Folge hat.

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Lebensereignis |Optional |

## Datensammlung

Die Klasse beschreibt die Metadaten des Ortes, an dem der Datensatz beschrieben wird, z. B. auf einem regionalen Portal für öffentliche Dienste und/oder einem nationalen eGovernment-Portal.

eCH-0200
Der Metadateneintrag einer Datensammlung (Metadateneintrag der Klasse „dcat:Dataset“) beschreibt eine einzelne, thematisch geschlossene Datensammlung, die von einer für den Inhalt verantwortlichen Stelle (Institution, Person) bereitgestellt wird. Die Datensammlung kann in unterschiedlichen Formen verfügbar sein (z.B. als Datei im Format text/csv oder als Datenbank mit Programmierschnittstelle). Jede Bereitstellungsform einer Datensammlung wird mittels eines Metadateneintrags der Klasse „dcat:Distribution“ beschrieben.   

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Datensammlung |Optional |

Die folgenden Unterabschnitte definieren die Attribute der Klasse Datensammlung.

### Identifikator

Dieses Attribut stellt den Identifikator einer Datensammlung dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
identifikator |dct:identifier |Text |1..1

### Herausgeber

Dieses Attribut steht für den Herausgeber der Datensammlung, d. h. für eine öffentliche Organisation, die für die Bereitstellung der Datensammlung verantwortlich ist.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
herausgeber |dct:publisher |Agent |1..1

### Name

Dieses Attribut stellt den Namen des Datensatzes dar. Dieses Attribut kann für parallele Sprachversionen des Namens wiederholt werden.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
name |dct:title |Text |1..n

### Landing Page

Dieses Attribut bezieht sich auf eine Webseite, die Zugang zur Datensammlung der öffentlichen Dienstleistung bietet. Sie soll auf eine Landing Page beim ursprünglichen Datenanbieter verweisen, nicht auf eine Seite auf der Website eines Dritten.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
landingPage |dcat:landingPage |Document |1..n

### Gehört zu

Verbindet eine Datensammlung zur öffentlichen Dienstleistung.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
gehörtZu |dcat:landingPage |Öffentliche Dienstleistung |0..n

## Beteiligung

Der CPSV-AP kennt eine Rolle im Zusammenhang mit öffentlichen Dienstleistungen, nämlich die der zuständigen Behörde. Diese einfache Struktur erlaubt es jedoch nicht, Aussagen über diese Teilnehmer zu machen, wie z.B. das Anfangs- und Enddatum eines Vertrages, und sie unterstützt auch nicht die Einbeziehung anderer Rollen. Die Klasse "Beteiligung" unterstützt diese zusätzliche Komplexität, falls erforderlich, z. B. die Beschreibung eines Dienstleistungsnutzers oder eines Dienstleistungsanbieters.

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Beteiligung |Optional |

Die folgenden Unterabschnitte definieren die Attribute der Klasse Beteiligung.

### Identifikator

Dieses Attribut stellt einen Identifikator der Klasse Beteiligung dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
identifikator |dct:identifier |Text |1..1

### Beschrieb

Dieses Attribut stellt einen Freitextbeschrieb der Klasse Beteiligung dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
beschrieb |dct:description |Text |1..1

### Rolle

Dieses Attribut gibt die Rolle an welche in der Beteiligung eingenommen wird. Dies sollte unter Verwendung eines kontrollierten Vokabulars erfolgen. Da es sich um einen Erweiterungsmechanismus für die CSPV-AP handelt, sollte das kontrollierte Vokabular so gewählt werden, dass es den lokalen Implementierungen entspricht. 

Attribut |URI |Range |Kardinalität
|---|---|---|---|
rolle |cv:role |Konzept |1..n

## Bedingung

Bedingung oder Voraussetzung zum Bezug einer öffentlichen Dienstleistung, die durch geeignete Nachweise zu belegen ist.

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Bedingung |Optional |

Die folgenden Unterabschnitte definieren die Attribute der Klasse Bedingung.

### Identifikator

Dieses Attribut stellt einen Identifikator der Klasse Bedingung dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
identifikator |dct:identifier |Text |1..1

### Name

Dieses Attribut stellt den Namen der Bedingung dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
name |dct:title |Text |1..1

### Art

Dieses Attribut stellt die Art der Bedingnung dar, wie sie in einem kontrollierten Vokabular beschrieben ist.  

Attribut |URI |Range |Kardinalität
|---|---|---|---|
art |dct:type |Konzept |0..n

### Erfüllt

Die Regeln, die die Bedingung erfüllt.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
 fulfils |dct:relation |Regel |0..*

### Hat Nachweis

Belege, die Informationen, Beweise oder Unterstützung für die Bedingung liefern.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
hatNachweis |dct:relation |Nachweis |0..n

## Nachweis

Ein Nachweis ist jedes Artefakt, das Informationen enthält, welche eine Entscheidung über die Erfüllung eines Kriteriums dokumentieren oder beweisen können. Im Zusammenhang mit Öffentlichen Dienstleistungen handelt es sich dabei meist um Verwaltungsdokumente oder ausgefüllte Antragsformulare. In manchen Fällen ist das Ergebnis einer öffentlichen Dienstleistung der Nachweis für eine andere öffentliche Dienstleistung.

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Nachweis |Optional |

Die folgenden Unterabschnitte definieren die Attribute der Klasse Nachweis.

### Identifikator

Dieses Attribut stellt einen Identifikator der Klasse Nachweis dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
identifikator |dct:identifier |Text |1..1

### Name

Dieses Attribut stellt den Namen eines Nachweises dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
name |dct:title |Text |1..1

### Beschrieb

Dieses Attribut stellt einen Freitextbeschrieb der Klasse Nachweis dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
beschrieb |dct:description |Text |0..1

### Art

Dieses Attribut stellt die Art der Bedingung dar, wie sie in einem kontrollierten Vokabular beschrieben ist.  

Attribut |URI |Range |Kardinalität
|---|---|---|---|
art |dct:type |Konzept |0..1

### Zugehörige Dokumentation

Dieses Attribut steht für die Dokumentation, die Informationen zu den Nachweisen enthält, z. B. eine bestimmte Vorlage für ein Verwaltungsdokument, eine Anwendung oder eine Anleitung zur Formatierung der Eingabe.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
zugehörigeDokumentation |foaf:page |Document |0..n

### Sprache

Gibt die Sprache(n) an, in der/denen die Nachweise erbracht werden müssen.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
sprache |dct:language |dct:LinguisticSystem |0..n

### Dient der Bedingung

Bedingung für die ein Nachweis als Beweis dient.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
dientDerBedingung |dct:language |dct:LinguisticSystem |0..n

## Ergebnis

Ein Ergebnis kann eine beliebige Ressource sein (ein Dokument, ein Artefakt), welche aus einer öffentlichen Dienstleistung entsteht. Meist stellt ein Ergebnis ein offizielles Dokument oder ein anderes Artefakt der zuständigen Behörde dar, das einen Beamten erlaubt/ermächtigt, etwas zu tun. In einigen Fällen wird das Ergebnis einer öffentlichen Dienstleistung als «Evidenz» für die Erfüllung eines Anforderungskriteriums einer anderen öffentlichen Dienstleistung verwendet. Solche Beziehungen sollten in den zugehörigen Regeln zu beschreiben.

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Ergebnis |Optional |

Die folgenden Unterabschnitte definieren die Attribute der Klasse Ergebnis.

### Identifikator

Dieses Attribut stellt einen Identifikator der Klasse Ergebnis dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
identifikator |dct:identifier |Text |1..1

### Name

Dieses Attribut stellt den Namen eines Ergebnis dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
name |dct:title |Text |1..1

### Beschrieb

Dieses Attribut stellt einen Freitextbeschrieb der Klasse Ergebnis dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
beschrieb |dct:description |Text |0..1

### Art

Dieses Attribut stellt die Art des Ergebnisses dar, wie sie in einem kontrollierten Vokabular beschrieben ist.  

Attribut |URI |Range |Kardinalität
|---|---|---|---|
art |dct:type |Konzept |0..n

## Gebühr

Die Klasse Gebühr steht für alle Kosten im Zusammenhang mit der Erbringung einer öffentlichen Dienstleistung, die die/der Empfänger einer Dienstleistung zu tragen hat.

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Gebühr |Optional |

Die folgenden Unterabschnitte definieren die Attribute der Klasse Gebühr.

### Identifikator

Dieses Attribut stellt den Identifikator der Klasse Gebühr dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
identifikator |dct:identifier |Text |1..1

### Wert

Dieses Attribut stellt einen numerischen Wert dar, der die Höhe der Gebühr angibt.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
wert |cv:value |Zahl |0..1

### Währung

Dieses Attribut stellt die Währung dar, in der die Gebühr bezahlt werden muss und der Wert der Gebühr ausgedrückt wird. Die möglichen Werte für Dieses Attribut werden in einem kontrollierten Vokabular beschrieben.  

Attribut |URI |Range |Kardinalität
|---|---|---|---|
währung |cv:currency |Konzept |0..1

### Beschrieb

Dieses Attribut stellt einen Freitextbeschrieb der Klasse Gebühr dar.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
beschrieb |dct:description |Text |0..1

### Ist definiert Durch

Dieses Attribut verknüpft die Klasse Gebühr mit einer oder mehreren Instanzen der Klasse Öffentliche Organisation. Dieses Attribut gibt an, welche öffentliche Organisation die zuständig für die Festlegung der Gebühr im Zusammenhang mit der Erbringung einer bestimmten öffentlichen Dienstleistung ist.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
istDefiniertDurch |cv:isDefinedBy |Öffentliche Organisation |0..n

### Wenn zugegriffen über

Wenn die Gebühren je nach verwendetem Kanal variieren, z. B. wenn der Zugriff über einen Online-Dienst erfolgt und nicht an einem physischen Ort, können die Gebühren mit dem Kanal verknüpft werden, indem das Attribut "Wenn der Zugriff über" verwendet wird.

|Attribut| URI| Range |Kardinalität|
|---|---|---|---|
|wennZugegriffenÜber|cv:ifAccessedThrough |Kanal|0..1|

## Kanal

Die Klasse "Kanal" stellt das Medium dar, über das eine öffentliche Dienstleistung angeboten wird, nutzt oder auf andere Weise mit ihr interagiert. Typische Beispiele sind Webportale, Schnittstellen, Telefon, Schalterservice usw.

|Klassenname |Obligatorisch/Optional|URI|
|---|---|---|
|Kanal |Optional |

Die folgenden Unterabschnitte definieren die Attribute der Klasse Kanal.

### Identifikator

Dieses Attribut stellt den Identifikator der Klasse Kanal dar.

|Attribut| URI |Range |Kardinalität|
|---|---|---|---|
|identifikator |dct:identifier |Text| 1..1|

### Gehört

Dieses Attribut verknüpft die Klasse Kanal mit einer oder mehreren Instanzen der Klasse Agent. Dieses Attribut gibt den Eigentümer eines bestimmten Kanals an, über den eine öffentlicher Dienstleistung bereitgestellt wird. Beachten Sie, dass öffentliche Organisation eine Unterklasse von Agent ist, so dass, wenn der Eigentümer die öffentliche Organisation ist, das Attribut «gehört» mit ihr verknüpft werden kann.

|Attribut| URI |Range| Kardinalität|
|---|---|---|---|
|gehört |cv:ownedBy |Öffentliche Organisation|0..n|

### Art

Dieses Attribut stellt die Art des Kanals dar, wie sie in einem kontrollierten Vokabular beschrieben ist.  

|Attribut |URI |Range |Kardinalität|
|---|---|---|---|
|art|dct:type|Konzept|0..1|

### Hat Input

In den meisten Fällen ist der für die Nutzung einer öffentlichen Dienstleistung erforderliche Nachweis unabhängig vom Kanal, über den auf die Dienstleistung zugegriffen wird. Das Attribut «Hat Input» sollte verwendet werden, um eine öffentliche Dienstleistung direkt mit einem oder mehreren Nachweisen zu verknüpfen. Wenn jedoch die Art des erforderlichen Nachweises je nach dem für den Zugriff auf die öffentliche Dienstleistung verwendeten Kanal variiert, kann das Attribut «Hat Input» auf Kanalebene verwendet werden. Beispielsweise kann für einen Online-Kanal eine digitale Signatur erforderlich sein, während für eine persönliche Dienstleistung eine physische Unterschrift erforderlich sein kann.

|Attribut |URI |Range| Kardinalität|
|---|---|---|---|
|hatInput| cpsv:hasInput|Nachweis| 0..n|

### Öffnungszeiten

Dieses Attribut steht für die normalen Öffnungszeiten eines Kanals. Der Wert sollte dem flexiblen Format folgen, das für die schema.org-Eigenschaft "opening hours " definiert wurde. Entsprechend dieser Struktur werden die Wochentage durch Codes mit zwei Buchstaben dargestellt (Mo, Di, We, Do, Fr, Sa, So). Die Listen sollten durch Kommata getrennt werden (z. B. Mo, We, Fr) und die Punkte durch einen Bindestrich (z. B. Mo-Fr).

Wenn es angebracht ist, Öffnungszeiten hinzuzufügen, dann folgt dies dem Tag, d. h. wenn ein Telefondienst von Montag bis Samstag von 08:00 bis 20:00 Uhr und sonntags von 08:00 bis 18:00 Uhr verfügbar ist, würde dies als Mo-Sa 08:00 bis 20:00 Uhr und So 08:00 bis 18:00 Uhr kodiert werden. 

|Attribut |URI |Range| Kardinalität|
|---|---|---|---|
|öffnungszeiten |schema:openingHours|Text|0..n|

### Einschränkung der Verfügbarkeit

Dieses Attribut verknüpft einen Kanal mit Informationen darüber, wann der Kanal nicht verfügbar ist, und setzt die allgemeinen Angaben zu den Öffnungszeiten ausser Kraft. Die Details werden über die Klasse "Öffnungszeiten " bereitgestellt.

|Attribut| URI |Range |Kardinalität|
|---|---|---|---|
|einschränkungDerVerfügbarkeit |schema:hoursAvailable|Öffnungszeiten|0..1|

## Öffnungszeiten

Die Klasse «Spezifikation der Öffnungszeiten» kann verwendet werden, um Angaben zu aussergewöhnlichen Umständen zu machen, wie z.B., dass das Unternehmen an Feiertagen geschlossen ist. Der CPSV-AP nutzt die Eigenschaft "openingHours" von schema.org , um Angaben zum regulären Betrieb zu machen.

|Klassenname| Obligatorisch/Optional |URI|
|---|---|---|
|Öffnungszeiten |Optional |

Keine Egenschaften definiert…..

The CPSV-AP makes use of schema.org’s openingHours Attribut to provide details of regular operations. The Opening Hours Specification class can be used to provide details of exceptional circumstances, such as being closed on public holidays, which is encoded (in Turtle), thus:
ex:PublicHolidayClosed a schema:OpeningHoursSpecification; schema:dayOfWeek <http://schema.org/PublicHoliday>.

Note that the Attribut schema:opens is not used, therefore the contact point is closed. More specific closures can be indicated by including the schema:validFrom and schema:validThrough properties, for example:
ex:ChristmasClosed a schema:OpeningHoursSpecification; schema:validFrom “2016-12-24T012:00Z”; schema:validThrough “2017-01-02T09:00Z”.

## Regel

Die Klasse "Regel" stellt ein Dokument dar, das die spezifischen Regeln, Richtlinien oder Verfahren festlegt, die bei öffentlichen Dienstleistungen zu befolgen sind. Dazu gehören unter anderem die Nutzungsbedingungen, Lizenz- und Authentifizierungsanforderungen der öffentlichen Dienstleistung.

|Klassenname |Obligatorisch/Optional|URI|
|---|---|---|
|Regel |Optional ||

Die folgenden Unterabschnitte definieren die Attribute der Klasse Regel.

### Identifikator

Dieses Attribut stellt den Identifikator für die Klasse Regel dar.

|Attribut |URI |Range |Kardinalität|
|---|---|---|---|
|identifikator |dct:identifier|Text|1..1|

### Beschrieb

Dieses Attribut stellt einen Freitextbeschrieb der Klasse Regel dar.

|Attribut |URI |Range|Kardinalität|
|---|---|---|---|
|beschrieb |dct:description|Text|1..1|

### Sprache

Dieses Attribut stellt die Sprache(n) dar, in der die Regel verfügbar ist. Dabei kann es sich um eine oder mehrere Sprachen handeln. Die möglichen Werte für Dieses Attribut werden in einem kontrollierten Vokabular beschrieben.

|Attribut|URI|Range|Kardinalität|
|---|---|---|---|
|sprache |dct:language |dct:LinguisticSystem |0..n|

### Name

Dieses Attribut stellt den Namen der Klasse Regel dar.

|Attribut|URI|Range |Kardinalität|
|---|---|---|---|
|name|dct:title|Text|1..1|

### Implementiert

Das Attribut implementiert, verknüpft eine Regel mit den relevanten Gesetzgebungs- oder Strategiedokumenten, d. h. mit der rechtlichen Ressource, unter der die Regeln definiert werden.

|Attribut |URI|Range |Kardinalität|
|---|---|---|---|
|implementiert |cpsv:implements |Öffentliche Dienstleistung|0..n|
## Agent 
Die Klasse «Agent» definiert jedes Subjekt, das handelt oder die Befugnis hat, zu handeln. Dazu gehören Personen, Organisationen und Gruppen. Die Klasse Öffentliche Organisation, ist eine wichtige Unterklasse von Agent.

|Klassenname |Obligatorisch/Optional|URI|
|---|---|---|
|Agent |Optional ||

Die folgenden Unterabschnitte definieren die Attribute der Klasse Agent.

### Name

Dieses Attribut stellt den Namen des Agenten dar.

|Attribut |URI|Range|Kardinalität|
|---|---|---|---|
|name|dct:title |Text|1..1|

### Identifikator

Dieses Attribut stellt den Identifikator für die Klasse Regel dar.

|Attribut|URI|Range |Kardinalität|
|---|---|---|---|
|identifikator|dct:identifier|Text |1..1|

### Hat Rolle

Dieses Attribut verknüpft einen Agenten mit der Klasse "Beteiligung". Die Klasse Beteiligung erleichtert den detaillierten Beschrieb der Art und Weise, wie ein Agent an einer öffentlichen Dienstleistung teilnimmt oder mit ihr interagiert, und kann zeitliche und räumliche Einschränkungen für diese Beteiligung enthalten.

|Attribut|URI |Range|Kardinalität|
|---|---|---|---|
|hatRolle |cv:playsRole|Beteiligung|0..n|

### Hat Adresse

Dieses Attribut steht für eine Adresse, die mit einem Agenten verbunden ist. Die Verbindung mit einer Adressbeziehung impliziert, dass der Agent eine Adresse hat.

|Attribut|URI |Range |Kardinalität|
|---|---|---|---|
|hatAdresse |cv:hasAddress |Adresse |0..1|

## Rechtsgrundlage

Diese Klasse stellt die Gesetze, Richtlinien, Weisungen oder Reglemente dar, die hinter den Regeln für die Dienstleistung stehen.

|Klassenname |Obligatorisch/Optional|URI|
|---|---|---|
|Rechtsgrundlage |Optional ||

Der folgende Unterabschnitt definiert das Attributeder Klasse Rechtsgrundlage.

### Verbunden

Dieses Attribut steht für eine andere Instanz der Klasse Rechtsgrundlage, die mit der beschriebenen Rechtsgrundlage in Beziehung steht.

|Attribut|URI|Range|Kardinalität|
|---|---|---|---|
|verbunden |dct:relation|Rechtsgrundlage|0..n|

## Organisation

Eine Gruppe von Menschen, die sich zu einer Gemeinschaft oder einer anderen sozialen, wirtschaftlichen oder politischen Struktur zusammengeschlossen hat. Die Gruppe hat einen gemeinsamen Zweck oder Grund für ihre Existenz, und kann als Agent fungieren. Organisationen sind oft in hierarchische Strukturen zerlegbar.

|Klassenname |Obligatorisch/Optional|URI|
|---|---|---|
|Organisation |Optional ||

## Öffentliche Organisation

Eine Organisation, die durch einen gesetzlichen Leistungsauftrag als Teil des öffentlichen Sektors (über sämtliche Föderalen Ebenen) definiert ist.

|Klassenname |Obligatorisch/Optional |URI|
|---|---|---|
|Öffentliche Organisation|Obligatorisch ||

Die folgenden Unterabschnitte definieren die Attribute der Klasse öffentliche Organisation.

### Bevorzugte  Bezeichnung

Eine bevorzugte Bezeichnung wird verwendet, um den primären, rechtlich anerkannten Namen der öffentlichen Organisation anzugeben, wie er in der ORG-Ontologie definiert ist. 

|Attribut |URI |Range|Kardinalität|
|---|---|---|---|
|bevorzugteBezeichnung|skos:prefLabel |Text|1..1|

### Räumliche Zuordnung

Dieses Attribut verbindet eine Organisation mit der/den Verwaltungsregion(en), die sie abdeckt.

|Attribut|URI|Range |Kardinalität|
|---|---|---|---|
|räumlicheZuordnung |dct:spatial|Location|1..n|

## Kontaktstelle

Diese Klasse stellt die Kontaktinformationen für eine öffentliche Dienstleistung, Kanal, eine öffentliche Organisation usw. dar.

|Klassenname|Obligatorisch/Optional|URI|
|---|---|---|
|Kontaktstelle |Optional ||

Der folgende Unterabschnitt definiert das Attribut der Klasse Kontaktstelle.

### Einschränkung der Verfügbarkeit

Dieses Attribut verknüpft eine Kontaktstelle mit Informationen darüber, wann die Kontaktstelle nicht verfügbar ist. Die Angaben werden über die Klasse Spezifikation der Öffnungszeiten bereitgestellt.

|Attribut |URI|Range |Kardinalität|
|---|---|---|---|
|einschränkungDerVerfügbarkeit |schema:hoursAvailable|Öffnungszeiten|0..n|

## Konzept

Die Klasse «Konzept» steht für jedes Konzept, das für die Klassifizierung einer öffentlichen Dienstleistung verwendet werden kann und das sich über die Eigenschaft "ist klassifiziert durch" auf sie bezieht. Sie dient dazu, Ergänzungen zur Klassifizierung einer öffentlichen Dienstleistung hinzuzufügen, die im CPSV-AP nicht explizit definiert wurden. Das Konzept kann zu einer bestimmten Sammlung (siehe Klasse «Sammlung) gehören oder nicht.

|Klassenname |Obligatorisch/Optional|URI|
|---|---|---|
|Konzept |Optional ||

## Sammlung

Diese Klasse stellt die Sammlung dar, zu der ein Konzept (Siehe Klasse Konzept) gehört. Sammlungen sind nützlich, wenn eine Gruppe von Konzepten etwas gemeinsam hat und es zweckmässig ist, sie unter einer gemeinsamen Bezeichnung zusammenzufassen, oder wenn einige Konzepte in eine sinnvolle Reihenfolge gebracht werden können.

|Klassenname|Obligatorisch/Optional|URI|
|---|---|---|
|Sammlung |Optional ||

Die folgenden Unterabschnitte definieren die Attribute der Klasse Sammlung.

### Mitglied

Das Attribut Mitglied, ermöglicht die Angabe der Konzepte, die Teil einer Sammlung sind.

|Attribut|URI|Range |Kardinalität|
|---|---|---|---|
|mitglied |skos:member|Konzept|0..n|

## Adresse

Strukturierte Informationen, die die eindeutige Bestimmung eines Objekts zum Zwecke der Identifizierung und Lokalisierung ermöglichen. "Identifizierung" bezieht sich darauf, dass die strukturierten Informationen in der Adresse das Objekt eindeutig bestimmen, d. h. sie helfen dem Menschen, das Objekt zu identifizieren. Mit anderen Worten: "Identifizierung" bezieht sich hier nicht auf eindeutige Bezeichner in einer Datenbank oder einem Datensatz. (ISO 19160-1:2015)

Klassenname |Obligatorisch/Optional |URI
|---|---|---|
Adresse |Optional |

Die folgenden Unterabschnitte definieren die Attribute der Klasse Adresse.

### Adressraum

Der Name eines geografischen Gebiets, in dem Adressen zusammengefasst werden.

|Attribut|URI|Range|Kardinalität|
|---|---|---|---|
|adressraum|dct:relation|Text|0..*|

### Adress ID

Ein weltweit eindeutiger Bezeichner für jede Instanz einer Adresse.

|Attribut|URI |Range |Kardinalität|
|---|---|---|---|
|adressID |dct:relation|String|0..*|

### Administrative Einheit

Die Beziehung administrative Einheit verknüpft eine Adresse mit der Klasse Verwaltungseinheit .

|Attribut|URI|Range|Kardinalität|
|---|---|---|---|
|administrativeEinheit |dct:relation|AdminUnit|0..*|

### Administrative Einheit Ebene 1

Der Name der obersten Ebene der Adresse, fast immer ein Kanton .

Attribut |URI |Range |Kardinalität
|---|---|---|---|
administrativeUnitLevel1 |dct:relation |Text |0..*

### Verwaltungseinheit Ebene 2

Der Name einer sekundären Ebene/Region der Adresse, in der Regel eine Gemeinde, ein Bezirk, ein   anderes Gebiet, das in der Regel mehrere Ortschaften umfasst.

|Attribut|URI |Range|Kardinalität|
|---|---|---|---|
|AdministrativeUnitLevel2|dct:relation|Text |0..*|

### Vollständige Adresse

Die vollständige Adresse in Form einer Zeichenkette.

|Attribut|URI|Range|Kardinalität|
|---|---|---|---|
| vollständigeAdresse |dct:relation |Text|0..*|

### Locator Designator

Eine Zahl oder Zeichenfolge, die den Locator innerhalb des betreffenden Bereichs eindeutig identifiziert.

|Attribut |URI|Range |Kardinalität|
|---|---|---|---|
 |locatorDesignator |dct:relation |String |0..*|

### Lokator Name

Namen für die durch den Locator identifizierte reale Entität.

|Attribut|URI |Range|Kardinalität|
|---|---|---|---|
 |locatorDesigantor|dct:relation|Text |0..*|

### Postleitzahl

Der Code, der für postalische Zwecke erstellt und gepflegt wird, um eine Unterteilung von Adressen und Postzustellungsstellen zu identifizieren.

|Attribut |URI |Range |Kardinalität|
|---|---|---|---|
 |postleitzahl |dct:relation |String |0..*|

### Postname Stadt

Ein Name, der für postalische Zwecke geschaffen und gepflegt wird, um eine Unterteilung von Adressen und Postzustellungsstellen zu identifizieren.

|Attribut |URI|Range |Kardinalität|
|---|---|---|---|
 |postnameStadt|dct:relation|Text|0..*|

### Postsfach

Eine Ortsbezeichnung für eine Postzustellungsstelle bei einem Postamt, in der Regel eine Nummer.

|Attribut|URI |Range|Kardinalität|
|---|---|---|---|
 |postfach|dct:relation|String|0..*|

### Durchgang

Bezeichnung für einen Durchgang oder eine Durchfahrt von einem Ort zum anderen.

|Attribut |URI |Range |Kardinalität|
|---|---|---|---|
 |durchgang |dct:relation|Text|0..*|

## Konzessionsvertag

Die Konzession beschreibt einen Vertrag zwischen öffentlichen Organisationen und einer oder mehreren Firmen. Ein Konzessionsvertrag verleiht dem Konzessionär das Recht, eine monopolisierte Tätigkeit aus­zuüben oder beinhaltet die Zuweisung einer öffentlichen Sache zur Sondernutzung.

|Klassenname|Obligatorisch/Optional|URI|
|---|---|---|
|Konzessionsvertrag |Optional ||

Die folgenden Unterabschnitte definieren die Attribute der Klasse Konzessionsvertrag.

### Beschrieb

Ein Freitextbeschrieb des Konzessionsvertrags.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
beschrieb |dct:relation |Text |1..*

### Eingeführt auf Grundlage von

Dieses Attribut verknüpft einen Konzessionsvertrag mit Rechtsvorschriften oder politischen Dokumenten , d. h. mit der Rechtsgrundlage, unter der die Konzessionsverträge festgelegt werden.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
eingeführtAufGrundlageVon |dct:relation |Rechtsgrundlage |0..*

### Hat öffentlichen Aufrtag

Sie verbindet einen Konzessionsvertrag mit der öffentlichen Organisation, die letztlich für eine öffentliche Dienstleistung verantwortlich ist.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
hatÖffentlichenAuftrag |dct:relation |Öffentliche Organisation |1..*

### hat Wirtschaftsbeteiligten  

Sie verbindet einen Konzessionsvertrag mit dem Wirtschaftsbeteiligten, der für die Bereitstellung und Verwaltung der öffentlichen Dienstleistungen zuständig ist.

Attribut |URI |Range |Kardinalität
|---|---|---|---|
hatWirtschaftsbeteiligten |dct:relation |Öffentliche Organisation |1..*

### Identifikator

Eindeutiger Verweis auf einen Konzessionsvertrag.

|Attribut|URI|Range|Kardinalität|
|---|---|---|---|
| identifikator|dct:relation|Literal|1|

## Vertrag

Zweiseitiges oder mehrseitiges Rechtsgeschäft, das durch Austausch von einander entsprechenden Willensäusserungen der Beteiligten, anhand einer bindenden Vereinbarung, zustande kommt. Obligationenrecht, Tit. vor Art. 1 (SR 220, Stand 2017-01)

|Klassenname |Obligatorisch/Optional |URI|
|---|---|---|
|Vertrag |Optional ||
