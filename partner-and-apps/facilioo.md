---
description: Anfragen schneller, transparenter und nachhaltiger Bearbeiten
---

# facilioo

## Übersicht

* **Kategorien**: [Eigentümerverwaltung](../kategorien/eigentuemerverwaltung.md), [Mieterkommunikation](../kategorien/mieterkommunikation.md), [Handwerkerportal & Auftragsmanagement](../kategorien/handwerkerportal-and-auftragsmanagement.md)
* **Use Cases**: [Stammdaten](facilioo.md#stammdaten)
* **Marketplace**: [facilioo](facilioo.md)
* **API Dokumentation**: [Link](https://developers.facilioo.de/reference/pagination)

## Beschreibung

facilioo erweitert die bestehenden Aareon Connect Produkte für die Wohnungswirtschaft und erfüllt die Bedürfnisse von Mietern, Mitgliedern und Mitarbeitern. Von Funktionen wie Vorgangsmanagement und Visualisierung von Verbräuchen bis Mieterkommunikation bietet facilioo eine Vielzahl von praxisnahen Lösungen. Bei weiteren Fragen zur Anbindung melden Sie sich direkt bei facilioo.

## Mit facilioo verbinden

1. Um einen facilioo-Use-Case zu nutzen benötigen Sie zur Aktivierung die **facilioo API Zugangsdaten**. Diese finden Sie folgendermaßen:
   1. **Username**
   2. **Passwort**
   3. **Environment**
2. Nachdem Sie Aareon Connect Kunde geworden sind, können Sie die verfügbaren **facilioo Integrationen innerhalb Ihres ERP-Systems** auswählen und aktivieren.

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](../use-cases/stammdaten.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

#### Entitäten

| ERP                                                            | facilioo                  |
| -------------------------------------------------------------- | ------------------------- |
| [Wirtschaftseinheiten](../entitaeten/wirtschaftseinheiten.md)  | Projekt (API Tenant)      |
| [Gebäude](../entitaeten/gebaeude.md)                           | Gebäude                   |
| [Gebäude](../entitaeten/gebaeude.md)                           | Eingang                   |
| [Verwaltungseinheiten](../kategorien/eigentuemerverwaltung.md) | Einheit                   |
| [Mietverträge](../entitaeten/mietvertraege.md)                 | Vertrag (Typ: Mieter)     |
| [Mieter](../entitaeten/mieter.md)                              | Partei (Typ: Mieter)      |
| [Eigentümerverträge](../entitaeten/eigentuemervertraege.md)    | Vertrag (Typ: Eigentümer) |
| [Eigentümer](../entitaeten/eigentuemer.md)                     | Partei (Typ: Eigentümer)  |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="165">Name</th><th width="450.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

#### Voraussetzungen

* Es werden nur Mieter mit einer hinterlegten E-Mail Adresse synchronisiert
  * Mietverträge von Mietern, die dies nicht erfüllen, werden ebenfalls nicht synchronisiert

### 2. Dokumente

#### Übersicht

* [Allgemeine Informationen](../use-cases/dokumente.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1303538867)

#### Entitäten

| ERP       | facilioo         |
| --------- | ---------------- |
| Ordner    | Dokumentenordner |
| Dokumente | Dokumente        |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="165">Name</th><th width="450.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

