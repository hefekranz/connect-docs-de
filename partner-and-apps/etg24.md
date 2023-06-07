---
description: Das Onlineportal für ganzheitlich Optimierung von Prozessen
---

# etg24

## Übersicht

* **Kategorien**: [Eigentümerverwaltung](../kategorien/eigentuemerverwaltung.md), [Mieterkommunikation](../kategorien/mieterkommunikation.md)&#x20;
* **Use Cases**: [Stammdaten](etg24.md#stammdaten)
* **Marketplace**: [etg24](https://marketplace.aareon.com/de/listings/etg24)
* **API Dokumentation**: [Link](https://api.etg24.de/dokumentation/)

## Beschreibung

etg24 ist das Onlineportal für Immobilienverwaltungen, die bereit dafür sind Prozesse ganzheitlich zu optimieren und gleichzeitig ihren Kunden modernen sowie begeisternden Service bieten möchten. Mithilfe der bereits langjährig im Verwalteralltag bewährten Cloud-Lösung ist es möglich, Arbeitsprozesse ins digitale Zeitalter zu heben. Verwaltungsmitarbeiter und Kunden benötigen für die Nutzung von etg24 nur einen Web-Browser oder die mobile App.

## Mit etg24 verbinden

1. Um einen EverReal Use Case zu nutzten, müssen Sie sich gegenüber der etg24 API authentifizieren. Hierzu benötigen Sie den **API Token**.
2. Nachdem sie Aareon Connect Kunde geworden sind, können sie die verfügbaren **etg24 Integrationen innerhalb Ihres ERP Systems** auswählen und aktivieren. Mehr Details dazu finden Sie hier[^1].

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](../use-cases/stammdaten.md)
* Feld Mapping (_kommt in Kürze_)

#### Entitäten

| ERP                                                            | etg24         |
| -------------------------------------------------------------- | ------------- |
| [Wirtschaftseinheiten](../entitaeten/wirtschaftseinheiten.md)  | Objektgruppen |
| [Gebäude](../entitaeten/gebaeude.md)                           | Objekte       |
| [Verwaltungseinheiten](../kategorien/eigentuemerverwaltung.md) | Einheiten     |
| [Mietverträge](../entitaeten/mietvertraege.md)                 | Mietvertrag   |
| [Mieter](../entitaeten/mieter.md)                              | Mieter        |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="165">Name</th><th width="450.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

#### Voraussetzungen

* Es werden nur Mieter mit einer hinterlegten E-Mail Adresse synchronisiert
  * Mietverträge von Mietern, die dies nicht erfüllen, werden ebenfalls nicht synchronisiert



[^1]: (Link zu ERP overview)
