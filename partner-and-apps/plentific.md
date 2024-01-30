---
description: Plentific hilft Immobilienverwaltungen und Wohnungsunternehmen
---

# Plentific

## Übersicht

* **Kategorien**: [Handwerkerportal & Auftragsmanagement](../kategorien/handwerkerportal-and-auftragsmanagement.md), [Mieterkommunikation](../kategorien/mieterkommunikation.md), [Objektübergabe](../kategorien/objektuebergabe.md)
* **Use Cases**: [Stammdaten](../use-cases/stammdaten.md)
* **Marketplace**: [Plentific](https://marketplace.aareon.com/de/listings/plentific)
* **API Dokumentation**: [Link](https://dev.plentific.com/api/client/latest)

## Beschreibung

Plentific ist ein Online-Marktplatz für Haus- und Immobilienbesitzer, der es Benutzern ermöglicht, mit geprüften Fachleuten in Kontakt zu treten und Angebote für verschiedene Arten von Projekten zu erhalten. Die Plattform deckt eine breite Palette von Dienstleistungen ab, von kleinen Reparaturen bis hin zu umfassenden Renovierungsarbeiten und Bauprojekten. Plentific bietet auch eine Projektmanagement-Software, die es Benutzern ermöglicht, ihre Projekte zu verwalten und mit den beauftragten Fachleuten zu kommunizieren. Die Plattform legt großen Wert auf Qualität und Zuverlässigkeit der Dienstleistungen und bietet eine 100% Geld-zurück-Garantie, falls die Arbeit nicht den Erwartungen entspricht. Plentific ist in mehreren europäischen Ländern tätig und hat eine breite Palette von Partnern, darunter führende Immobilienunternehmen und Finanzinstitute.

## Mit Plentific verbinden

1.  Um einen Plentific-Use-Case zu nutzen benötigen Sie zur Aktivierung die **Plentific API-Schlüssel**. Diese finden Sie folgendermaßen:

    1. Klicken Sie auf **Konto** > **API-Schlüssel**
    2. Hier können Sie ihre **Client id** und **Client secret** einsehen oder neu rotieren.



    <figure><img src="../.gitbook/assets/image (2) (1).png" alt="" width="563"><figcaption><p>Plentific API Schlüssel</p></figcaption></figure>
2. Nachdem Sie Aareon Connect Kunde geworden sind, können Sie die verfügbaren **Plentific Integrationen innerhalb Ihres ERP-Systems** auswählen und aktivieren.

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](../use-cases/stammdaten.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

#### Entitäten

| ERP                                                            | Plentific                     |
| -------------------------------------------------------------- | ----------------------------- |
| [Gebäude](../entitaeten/gebaeude.md)                           | Objekte                       |
| [Verwaltungseinheiten](../kategorien/eigentuemerverwaltung.md) | Unterobjekte                  |
| [Mieter](../entitaeten/mieter.md)                              | Unterobjekte (Typ: Mieter)    |
| [Eigentümer](../entitaeten/eigentuemer.md)                     | Unterobjekte (Typ: Vermieter) |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="165">Name</th><th width="450.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

#### Voraussetzungen

* Es werden nur Mieter mit einer hinterlegten E-Mail Adresse synchronisiert
  * Mietverträge von Mietern, die dies nicht erfüllen, werden ebenfalls nicht synchronisiert

### 2. Tickets - In Bearbeitung

#### Übersicht

* [Allgemeine Informationen](../use-cases/tickets.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=388591826\&fvid=1169857418)
