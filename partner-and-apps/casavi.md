---
description: casavi ist die maßgeschneiderte Lösung für Ihr Wohnungsunternehmen
---

# casavi

## Übersicht

* **Kategorien**: [Handwerkerportal & Auftragsmanagement](../kategorien/handwerkerportal-and-auftragsmanagement.md), [Eigentümerverwaltung](../kategorien/eigentuemerverwaltung.md), [Mieterkommunikation](../kategorien/mieterkommunikation.md)
* **Use Cases**: [Stammdaten](../use-cases/stammdaten.md)
* **Marketplace**: [casavi](https://marketplace.aareon.com/listings/casavi)
* **API Dokumentation**: [Link](https://api.mycasavi.com/v2/docs/manager)

## Beschreibung

casavi ist die zentrale Plattform für die Digitalisierung Ihrer Wohnungsverwaltung. Transparentes und automatisiertes Vorgangsmanagement, ein moderner Markenauftritt, elektronischer Briefversand und die Zentralisierung der Kommunikation innerhalb Ihrer Liegenschaften sind die Grundlage unserer Lösung. Bei weiteren Fragen zur Anbindung melden Sie sich direkt bei casavi.

## Mit casavi verbinden

1. Um einen casavi-Use-Case zu nutzen benötigen Sie zur Aktivierung die **casavi API Zugangsdaten**. Diese finden Sie folgendermaßen:
   1. Klicken Sie auf **Administration** > **API-Zugangsdaten**&#x20;
   2. Hier können Sie ein neues Paar **Schlüssel** und **Secret** generieren oder ein existierendes Paar nutzen.

<figure><img src="../.gitbook/assets/casavi screenshot-1.png" alt="" width="563"><figcaption><p>casavi API Zugansdaten</p></figcaption></figure>

2. Nachdem sie Aareon Connect Kunde geworden sind können sie die verfügbaren **casavi Integrationen innerhalb Ihres ERP Systems** auswählen und aktivieren.

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](../use-cases/stammdaten.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1fLwCGcttemtlDpznO3O00352cZZ5SPJXBPv6IRWQ6Bk/edit?gid=1022321755#gid=1022321755)

#### Entitäten

| ERP                                                            | casavi                    |
| -------------------------------------------------------------- | ------------------------- |
| [Wirtschaftseinheiten](../entitaeten/wirtschaftseinheiten.md)  | Liegenschaften            |
| [Gebäude](../entitaeten/gebaeude.md)                           | Adressen                  |
| [Verwaltungseinheiten](../kategorien/eigentuemerverwaltung.md) | Einheiten                 |
| [Mietverträge](../entitaeten/mietvertraege.md)                 | Vertrag (Typ: Mieter)     |
| [Mieter](../entitaeten/mieter.md)                              | Kontakt (Typ: Mieter)     |
| [Eigentümervertrag](../entitaeten/eigentuemervertraege.md)     | Vertrag (Typ: Eigentümer) |
| [Eigentümer](../entitaeten/eigentuemer.md)                     | Kontakt (Typ: Eigentümer) |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="165">Name</th><th width="450.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

#### Voraussetzungen

* Es werden nur Mieter mit einem hinterlegten Nachnamen synchronisiert
* Es werden nur Stammdaten synchronisiert, welche mit einem Mieter verknüpft sind
  * Beispiel: Ein Wohnung welche leer ist, wird nicht synchronisiert
