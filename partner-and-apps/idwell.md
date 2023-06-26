---
description: iDWELL revolutioniert die Servicequalität im Immobilienmanagement
---

# iDWELL

## Übersicht

* **Kategorien**: [Eigentümerverwaltung](../kategorien/eigentuemerverwaltung.md), [Mieterkommunikation](../kategorien/mieterkommunikation.md)
* **Use Cases**: [Stammdaten](idwell.md#stammdaten)
* **Marketplace**: [iDWELL](https://marketplace.aareon.com/de/listings/idwell)
* **API Dokumentation**: [Link](https://api.docs.idwell.com/docs/public-api/f125ebad8f979-i-dwell-api)

## Beschreibung

iDWELL hat sich zum Ziel gesetzt, den Digitalisierungstrend in die traditionsreiche Immobilienbranche zu übersetzen und Unternehmen aktiv zu unterstützen, aufwändige Prozesse zu automatisieren. Die durchdachte Softwarelösung schafft Klarheit zwischen Immobilienverwaltungen, MieterInnen/EigentümerInnen und Dienstleistern.

## Mit iDWELL verbinden

1. Um einen iDWELL-Use-Case zu nutzen, müssen Sie sich gegenüber der **iDWELL** **API** authentifizieren. Hierzu benötigen Sie:
   1. **Benutzername**
   2. **Password**
   3. **Subdomain**: \
      Die Subdomain finden Sie, wenn Sie in Ihrem iDWELL Account eingeloggt sind oben in der URL Leiste. Hier wird ein Link mit folgender Anfangsstruktur zu sehen sein: [https://_**aareon-connect**_.idwell.com/](https://di-test.idwell.com/) Dort wo im Beispiel aareon-connect in fett und kursiv steht finden Sie Ihre Subdomain.
2. Nachdem Sie Aareon Connect Kunde geworden sind, können Sie die verfügbaren **iDWELL Integrationen innerhalb Ihres ERP-Systems** auswählen und aktivieren. Mehr Details dazu finden Sie hier[^1].

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](../use-cases/stammdaten.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

#### Entitäten

| ERP                                  | iDWELL    |
| ------------------------------------ | --------- |
| [Gebäude](../entitaeten/gebaeude.md) | Gebäude   |
| [Mieter](../entitaeten/mieter.md)    | Ersteller |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th>Name</th><th width="549.3333333333333">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

#### Voraussetzungen

* Es werden nur Mieter mit einer hinterlegten E-Mail Adresse synchronisiert
  * Mietverträge von Mietern, die dies nicht erfüllen, werden ebenfalls nicht synchronisiert

[^1]: (Link zu ERP overview)
