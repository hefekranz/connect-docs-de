# UTS KARTHAGO

## Schnittstelle

Je Partnersystem sollte ein separater API Benutzer erstellt werden, damit im ERP selber konfiguriert werden kann, welches Partnersystem welche Daten erhalten soll.

Mehr Details finden Sie im UTS KARTHAGO Handbuch.

## Use Cases

### Allgemein

* Bei allen Use Cases werden die Mandanten direkt im ERP System für die Schnittstelle freigegeben.\
  Deswegen, gibt es bei den UTS KARTHAGO Integrationen keine Mandanten Filterung bei der Aareon Connect Aktivierung selber.
* In UTS KARTHAGO gibt es keine Wirtschaftseinheiten, entsprechend sind alle Einstellungen dazu in allen Use Cases für UTS KARTHAGO irrelevant

### Stammdaten

#### Entitäten

| Aareon Connect Standard                                        | UTS KARTHAGO |
| -------------------------------------------------------------- | ------------ |
| [Wirtschaftseinheiten](../entitaeten/wirtschaftseinheiten.md)  | N/A          |
| [Gebäude](../entitaeten/gebaeude.md)                           | Objekte      |
| [Verwaltungseinheiten](../kategorien/eigentuemerverwaltung.md) | Einheiten    |
| [Mietverträge](../entitaeten/mietvertraege.md)                 | Verträge     |
| [Mieter](../entitaeten/mieter.md)                              | Mieter       |
| [Eigentümerverträge](../entitaeten/eigentuemervertraege.md)    | Verträge     |
| [Eigentümer](../entitaeten/eigentuemer.md)                     | Eigentümer   |

#### Besonderheiten

* Mietkosten werden bei UTS KARTHAGO nicht übertragen, entsprechend sind alle Einstellungen dazu für UTS KARTHAGO irrelevant

### Dokumente

#### Entitäten

| Aareon Connect Standard | UTS KARTHAGO |
| ----------------------- | ------------ |
| Archive                 | N/A          |
| Ordner                  | Ordner       |
| Dokumente               | Dokumente    |

#### Besonderheiten

* Nicht synchronisiert werden Dokumente, die
  * mit Adressen verknüpft sind
  * keine Ordnerzuordnung haben
  * größer als 50MB sind ([allgemeine Einschränkung des Dokumenten Use Cases](../use-cases/dokumente.md#einschraenkungen) für alle ERPs)
* Der Freigabestatus von Dokumenten wird aktuell nicht übermittelt, stattdessen werden alle synchronisierten Dokumente werden als "nicht freigegeben" behandelt
