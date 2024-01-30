---
description: KIWI - das digitale Schließsystem für die Wohnungswirtschaft
---

# KIWI

## Übersicht

* **Kategorien**: [Zugangsmanagement](../kategorien/zugangsmanagement.md)
* **Use Cases**: [Stammdaten](kiwi.md#stammdaten)
* **Marketplace**: [KIWI](https://marketplace.aareon.com/de/listings/kiwi)

## Beschreibung

KIWI bietet einfachen digitalen Zugang für Mehrfamilienhäuser. Wir machen physische Schlüssel für Wohnungsbaugesellschaften für alle Türen und Anwendungsfälle überflüssig und reduzieren so die Kosten, während wir gleichzeitig die Sicherheit und den Komfort erhöhen.

## Mit KIWI verbinden

1. Um einen KIWI Use Case zu nutzen müssen Sie sich gegenüber der **KIWI API** authentifizieren. Hierzu benötigen Sie:
   1. **Benutzername**
   2. **Password**
2. Nachdem Sie Aareon Connect Kunde geworden sind, können Sie die verfügbaren **KIWI Integrationen innerhalb Ihres ERP-Systems** auswählen und aktivieren.

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](../use-cases/stammdaten.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

#### Entitäten

| ERP                                                            | KIWI             |
| -------------------------------------------------------------- | ---------------- |
| [Verwaltungseinheiten](../kategorien/eigentuemerverwaltung.md) | _Kommt in Kürze_ |
| [Mietverträge](../entitaeten/mietvertraege.md)                 | _Kommt in Kürze_ |
| [Mieter](../entitaeten/mieter.md)                              | _Kommt in Kürze_ |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="165">Name</th><th width="450.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

#### Voraussetzungen

* Es werden nur Mieter mit einer hinterlegten E-Mail Adresse synchronisiert
  * Mietverträge von Mietern, die dies nicht erfüllen, werden ebenfalls nicht synchronisiert
