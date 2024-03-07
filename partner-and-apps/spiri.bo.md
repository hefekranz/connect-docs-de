---
description: >-
  Die Mieter-App der Wohnungswirtschaft. Spiri.Bo digitalisiert Ihren
  Kundenservice.
---

# Spiri.Bo

## Übersicht

* **Kategorien**: [Mieterkommunikation](../kategorien/mieterkommunikation.md)
* **Use Cases**: [Stammdaten](spiri.bo.md#stammdaten), [Tickets](../use-cases/tickets.md)
* **Marketplace**: [Spiri.Bo](https://marketplace.aareon.com/de/listings/spiribo)
* **API Dokumentation**: [Link](https://api.spiri.bo/v1/docs/silo#tag/building)

## Beschreibung

Spiri.Bo ist ein PropTech-Unternehmen der meravis Immobiliengruppe. Spiri.Bo digitalisiert die Wohnungswirtschaft für Mieterservice der begeistert. Spiri.Bo's Kern-Produkt ist die Spiri.Bo Mieterapp als All-In-One-Lösung:

## Mit Spiri.Bo verbinden

1. Um einen Spiri.Bo-Use-Case zu nutzen benötigen Sie zur Aktivierung die **Spiri.Bo API Zugansdaten**. Diese erhalten Sie folgendermaßen:
   1. Fordern Sie per Email an [dev+api-key@spiri.bo](mailto:dev+api-key@spiri.bo) mit dem Betreff "API-Key Aareon Connect" und Inhalt "Hallo, bitte sendet mir einen API-Key für Aareon Connect zu. Vielen Dank" den API Key an.&#x20;
2. Nachdem Sie Aareon Connect Kunde geworden sind, können Sie die verfügbaren **Spiri.Bo Integrationen innerhalb Ihres ERP-Systems** auswählen und aktivieren.

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](spiri.bo.md#stammdaten)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

#### Entitäten

| ERP                                                           | Spiri.Bo      |
| ------------------------------------------------------------- | ------------- |
| [Gebäude](../entitaeten/gebaeude.md)                          | Gebäude       |
| [Verwaltungseinheiten](../entitaeten/verwaltungseinheiten.md) | Wohnungen     |
| [Mietverträge](../entitaeten/mietvertraege.md)                | Verträge      |
| [Mieter](../entitaeten/mieter.md)                             | Mieterbestand |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="151">Name</th><th width="487.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr><tr><td>Nur Hauptmieter übertragen</td><td>Es werden nur Hauptmieter übertragen</td><td></td></tr></tbody></table>

#### Voraussetzungen

* Es werden nur Mieter mit einem hinterlegten Nachnamen synchronisiert
* Es werden nur Stammdaten synchronisert, welche mit einem Mieter verknüpft sind
  * Beispiel: Ein Wohnung welche leer ist, wird nicht synchronisert

#### Wohnungstypen Mapping

Die im ERP hinterlegt Nutzungsart (des Mietvertrags) wird wie folgt auf die Wohnungstypen in Spiri.Bo gemappt:

| ERP                          | Spiri.Bo   |
| ---------------------------- | ---------- |
| Wohnraum                     | living     |
| Wohnung                      | living     |
| Praxis                       | commercial |
| Einzelhandel                 | commercial |
| Büro                         | commercial |
| Gastronomie                  | commercial |
| Pflegedienst                 | commercial |
| Werkstatt                    | commercial |
| Gewerbe                      | commercial |
| Produktion                   | commercial |
| Logistik                     | commercial |
| gewerbliche Nutzung          | commercial |
| Garagen                      | parking    |
| Stellplatz außen             | parking    |
| Carport                      | parking    |
| Tiefgarage                   | parking    |
| Fahrradraum                  | parking    |
| Hochgarage                   | parking    |
| Garage                       | parking    |
| Lager                        | storage    |
| _Alle anderen Nutzungsarten_ | other      |

{% hint style="info" %}
Da die Nutzungsart im ERP System frei definierbar ist, wird das Mapping laufend erweitert.
{% endhint %}

### 2. Tickets

#### Übersicht

* [Allgemeine Informationen](../use-cases/tickets.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=388591826\&fvid=1169857418)

Die Aareon Connect Integration für das Übertragen von Meldungen aus Spiri.bo ins ERP besteht us 4 Komponenten:

1.  **Meldungskategorien und -typen Synchronisation**

    Dieser Teil muss initial aktiviert werden, um die Kategorien und Typen von Meldungen aus dem ERP an Spiri.bo zu übergeben. Es werden die Kategorien und Typen aus dem ERP abgeholt und per Mail an Spiri.bo weitergeleitet. Dort werden sie anschließend hinterlegt.
2. **Claims/Meldungen Synchronisation**\
   Nachdem die Kategorien und Typen in Spiri.bo angelegt wurden, kann dieser und alle weiteren Teile (3 & 4) aktiviert werden. In diesem Teil der Integration werden die Schadensmeldungen an das ERP weitergeleitet und erscheinen dort als Meldung.
3. **Forms Synchronisation**\
   Dieser Teil der Integration synchronisiert neu angelegte Formulare (Anfragen, Lärmbeschwerden, etc.) aus Spiri.bo in das ERP.
4. **Update Kontakt Informationen**\
   Der letzte Teil der Integration leitet Änderungen von Kontaktinformationen (Telefonnummern) aus Spiri.bo an das ERP weiter.&#x20;

**Einstellungen**

Sie müssen keine weiteren Einstellungen vornehmen.

**Voraussetzungen**

Damit die Synchronisation von Meldungen, Formularen und Kontaktänderungen im ERP ankommen, muss Teil 1 ("_Meldungskategorien und -typen Synchronisation_") aus der Übersicht erfüllt sein.

**Achtung**

Je nach Einstellung im ERP kann es vorkommen, dass Meldungen nicht direkt angezeigt werden. Fragen Sie hierzu Ihren ERP berater, wie häufig temporäre Meldungen temporäre Meldungen aus der Datenbank ins ERP übertragen werden.



### 3. Dokumente

#### Übersicht

* [Allgemeine Informationen](../use-cases/dokumente.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1303538867\&fvid=677380363)

#### Entitäten

| ERP       | Spiri.Bo  |
| --------- | --------- |
| Archive   | N/A       |
| Ordner    | N/A       |
| Dokumente | Dokumente |

#### Einstellungen

Im Zuge der Aktivierung des Dokumenten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="151">Name</th><th width="487.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Relevante Archiv IDs </td><td>IDs der Archive von welchen Dokumente übertragen werden sollen. </td><td></td></tr><tr><td>Wirtschaftseinheits Index ID</td><td>Index ID der Wirtschaftseinheitsnummer. </td><td></td></tr><tr><td>Gebäude Index ID</td><td>Index ID der Gebäudenummer. </td><td></td></tr><tr><td>Verwaltungseinheits Index ID</td><td>Index ID der Verwaltungseinheitsnummer. </td><td></td></tr><tr><td>Mietvertrags Index ID</td><td>Index ID der Mietvertragsnummer. </td><td></td></tr></tbody></table>

#### Voraussetzungen

* Indexe für Stammdatennummern müssen gesetzt sein

#### Besonderheiten

* Der Use Case enthält 2 Integrationen die beide aktiviert werden müssen&#x20;

