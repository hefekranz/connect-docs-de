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

| ERP                                                         | iDWELL             |
| ----------------------------------------------------------- | ------------------ |
| [Gebäude](../entitaeten/gebaeude.md)                        | Gebäude            |
| [Verwaltungseinheit](../entitaeten/verwaltungseinheiten.md) | Verwaltungseinheit |
| [Mieter](../entitaeten/mieter.md)                           | Mieter             |
| [Eigentümer](../entitaeten/eigentuemer.md)                  | Eigentümer         |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="187">Name</th><th width="549.3333333333333">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Mandanten Nummern Filtern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr><tr><td>Objekt Nummern Filtern</td><td>Es werden nur Daten für die eingetragenen Objekte synchronisiert.</td><td></td></tr></tbody></table>

#### Test der Integration: Stammdaten von ERP nach iDWELL

Nachdem Sie die Integration aktiviert haben und die ersten Stammdaten in Ihrem iDWELL Account zusehen sind, prüfen Sie bitte, ob alle Daten wie gewünscht übertragen wurden. Die verfügbaren Felder für ihr ERP und iDWELL finden Sie [**hier**](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279). Prüfen Sie die Entitäten folgendermaßen:

**Objekte**

Bitte überprüfen Sie, ob die übertragenen Informationen in den Reitern Info, Einheiten und Kunden korrekt übertragen wurden.

**Einheiten**

Bitte überprüfen Sie, ob die übertragenen Informationen in den Reitern Info, Kunden und Adresse korrekt übertragen wurden. Historische Mieter mit abgelaufenen Mietverträgen werden auch aus dem ERP nach iDWELL übertragen. Jedoch erhalten sie den Status "blocked" und sind nur zu sehen, wenn Sie dies in den Einstellungen anpassen. Dazu müssen Sie oben rechts auf das Dropdown-Menu clicken und dann weiter zum Reiter Unternehmen, welcher mit einem Zahnrad versehen ist. Hier können Sie die Einstellungen unter "Historie der archivierten Nutzer" vornehmen.

**Mieter/Eigentümer**

Bitte überprüfen Sie bei den Mietern, sowie Eigentümern, die Reiter Kontaktdaten, Info und Einheiten.



[^1]: (Link zu ERP overview)
