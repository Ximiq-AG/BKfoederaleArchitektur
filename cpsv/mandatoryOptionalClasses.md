# Obligatorische und optionale Klassen und Attribute von CPSV-AP

Um die Mindestanforderungen zur Erfüllung der CPSV-AP anzugeben, werden die Klassen und Attribute als obligatorisch oder optional klassifiziert. Eine Minimalimplementierung des CPSV-AP liefert Informationen über die obligatorischen Attribute der obligatorischen Klassen. Optionale Klassen können weiterhin obligatorische Attribute haben, für die Informationen bereitgestellt werden sollten, wenn die jeweilige Klasse im Beschrieb der öffentlichen Dienstleistungen verwendet wird.

Die Begriffe obligatorische Klasse, optionale Klasse, obligatorische Attribute und optionale Attribute haben die folgende Bedeutung:

- **Obligatorische Klasse**: Ein Empfänger von Daten MUSS in der Lage sein, Informationen über Instanzen der Klasse zu verarbeiten; ein Sender von Daten MUSS Informationen über Instanzen der Klasse liefern.

- **Optionale Klasse**: Ein Empfänger MUSS in der Lage sein, Informationen über Instanzen der Klasse zu verarbeiten; ein Sender KANN die Informationen bereitstellen, muss aber nicht.

- **Obligatorische Attribute**: Ein Empfänger MUSS in der Lage sein, die Informationen für dieses Attribut zu verarbeiten; ein Sender MUSS die Informationen für dieses Attribut bereitstellen. Falls die entsprechende Klasse als optional eingestuft ist, MUSS ein Empfänger in der Lage sein, die Informationen für dieses Attribut zu verarbeiten; ein Sender MUSS die Informationen für dieses Attribut bereitstellen, wenn er die entsprechende Klasse verwendet.

- **Optionale Attribut**: Ein Empfänger MUSS in der Lage sein, die Informationen für dieses Attribut zu verarbeiten; ein Sender KANN die Informationen für diese Eigenschaft bereitstellen, wenn sie verfügbar ist.

Die folgende Liste gibt einen Überblick darüber, welche Klassen und Attribute als obligatorisch oder optional eingestuft werden:

|Klasse|Attribut|Obligatorisch/optional|
|---|---|---|
|Öffentliche Dienstleistung | |  Obligatorisch |
|Öffentliche Dienstleistung |Identifikator|  Obligatorisch |
|Öffentliche Dienstleistung  |Name | Obligatorisch |
|Öffentliche Dienstleistung  |Beschrieb | Obligatorisch |
|Öffentliche Dienstleistung  |Schlüsselwort | Optional |
|Öffentliche Dienstleistung  |Sektor | Optional |
|Öffentliche Dienstleistung  |Themengebiet|Optional |
|Öffentliche Dienstleistung  |Art | Optional |
|Öffentliche Dienstleistung  |Sprache | Optional |
|Öffentliche Dienstleistung  |Status  |Optional |
|Öffentliche Dienstleistung  |Ist gruppiert nach| Optional |
|Öffentliche Dienstleistung  |Bedingt| Optional |
|Öffentliche Dienstleistung  |Ist verbunden mit | Optional |
|Öffentliche Dienstleistung  |Hat Bedingung |Optional |
|Öffentliche Dienstleistung  |Ist zuständig| Obligatorisch |
|Öffentliche Dienstleistung  |Hat Beteiligung| Optional |
|Öffentliche Dienstleistung  |Hat Input | Optional |
|Öffentliche Dienstleistung  |Hat Rechtsgrundlage| Optional |
|Öffentliche Dienstleistung  |Erzeugt| Optional |
|Öffentliche Dienstleistung  |Folgt |Optional |
|Öffentliche Dienstleistung  |Räumliche Zuordnung| Optional |
|Öffentliche Dienstleistung  |Hat Kontaktstelle| Optional |
|Öffentliche Dienstleistung  |Kanal |Optional |
|Öffentliche Dienstleistung  |Bearbeitungszeit| Optional |
|Öffentliche Dienstleistung  |Hat Gebühr |Optional |
|Öffentliche Dienstleistung  |Ist beschrieben in| Optional |
|Öffentliche Dienstleistung  |Ist klassifiziert durch| Optional |
|Ereignis ||  Optional |
|Ereignis | Identifikator | Obligatorisch |
|Ereignis  |Name | Obligatorisch |
|Ereignis | Beschrieb  |Optional |
|Ereignis | Art  |Optional |
|Ereignis | Verbundene Dienstleistung |Optional |
|Geschäftsereignis ||  Optional |
|Lebensereignis  || Optional |
|Datensammlung   || Optional |
|Datensammlung  |Identifikator | Obligatorisch |
|Datensammlung | Name  |Obligatorisch |
|Datensammlung | Herausgeber| Obligatorisch |
|Datensammlung | Landing Page | Obligatorisch |
|Beteiligung   ||Optional |
|Beteiligung  |Identifikator  |Obligatorisch |
|Beteiligung  |Beschrieb | Obligatorisch |
|Beteiligung  |Rolle | Obligatorisch |
|Bedingung ||  Optional |
|Bedingung  |Identifikator  |Obligatorisch |
|Bedingung | Name | Obligatorisch |
|Bedingung | Art | Optional |
|Nachweis ||  Optional |
|Nachweis | Identifikator | Obligatorisch |
|Nachweis | Name  |Obligatorisch |
|Nachweis  |Beschrieb | Optional |
|Nachweis | Art  |Optional |
|Nachweis | Zugehörige Dokumentation| Optional |
|Nachweis | Sprache | Optional |
|Ergebnis ||  Optional |
|Ergebnis  Identifikator  Obligatorisch |
|Ergebnis | Name  |Obligatorisch |
|Ergebnis | Beschrieb | Optional |
|Ergebnis|  Art  |Optional |
|Gebühr  ||  Optional |
|Gebühr  |Identifikator  |Obligatorisch |
|Gebühr  |Wert |Optional |
|Gebühr | Währung |Optional |
|Gebühr | Beschrieb  |Optional |
|Gebühr | Ist definiert durch |Optional |
|Gebühr | Wenn zugegriffen über |Optional |
|Kanal  ||  Optional |
|Kanal  |Identifikator | Obligatorisch |
|Kanal | Gehört |Optional |
|Kanal | Art | Optional |
|Kanal | Hat Input | Optional |
|Kanal  |Öffnungszeiten |Optional |
|Kanal | Einschränkung der Verfügbarkeit| Optional |
|Öffnungszeiten ||  Optional |
|Regel ||  Optional |
|Regel | Identifikator | Obligatorisch |
|Regel  |Beschrieb | Obligatorisch |
|Regel | Sprache | Optional |
|Regel  |Name | Obligatorisch |
|Regel | Implementiert| Optional |
|Rechtsgrundlage  || Optional |
|Rechtsgrundlage| Verbunden |Optional |
|Agent ||  Optional |
|Agent  |Identifikator  |Obligatorisch |
|Agent | Name  |Obligatorisch |
|Agent | Hat Rolle |Optional |
|Agent | Hat Adresse |Optional |
|Public Organisation  || Obligatorisch |
|Öffentliche Organisation | Bevorzugte Bezeichnung| Obligatorisch |
|Öffentliche Organisation  |Räumliche Zuordnung |Obligatorisch |
|Kontaktstelle ||  Optional |
|Konzept  || Optional |
|Sammlung ||  Optional |
|Sammlung| Mitglied| Optional |
|Organisation ||  Optional |
|Vertrag  || Optional |
|Konzessionsvertrag ||  Optional |
|Konzessionsvertrag| Beschrieb | Obligatorisch |
|Konzessionsvertrag |Identifikator | Obligatorisch |
|Konzessionsvertrag| Name | Obligatorisch |
|Konzessionsvertrag| Sprache | Optional |
|Konzessionsvertrag |Art | Optional |
|Adresse  || Optional |
|Adresse |Adressraum |Optional |
|Adresse |Adress ID| Optional |
|Adresse| Administrative Einheit| Optional |
|Adresse |Administrative Einheit Ebene 1| Optional |
|Adresse| Administrative Einheit Ebene 2 |Optional |
|Adresse |Vollständige Adresse| Optional |
|Adresse |Locator Designator| Optional |
|Adresse |Locator Name |Optional |
|Adresse |Postfach| Optional |
|Adresse| Postleitzahl |Optional |
|Adresse |Postname Stadt| Optional |
|Adresse |Durchgang|Optional |
