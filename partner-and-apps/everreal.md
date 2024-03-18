---
description: Die digitale B2B Software für Immobilienvermietung & Verkauf
---

# EverReal

## Übersicht

* **Kategorien**: [Interessentenmanagement](../kategorien/interessentenmanagement.md), [Objektübergabe](../kategorien/objektuebergabe.md), [Reporting](../kategorien/reporting.md)
* **Use Cases**: [Stammdaten](../use-cases/stammdaten.md)
* **Marketplace**: [EverReal](https://marketplace.aareon.com/de/listings/everreal)
* **API Dokumentation**: [Link](https://api-docs.everreal.co/endpoints)

## Beschreibung

EverReal ist eine professionelle B2B Software für digitalen Mieterwechsel und Verkauf. Unsere cloudbasierte, modulare Lösung deckt den kompletten Prozess vollständig digital ab, von der Vermarktung über Interessenten- und Bewerbermanagement bis hin zur Vertragsunterzeichnung und Wohnungsübergabe und spart Ihnen bis zu 80% Zeit. Ideal für Immobilienunternehmen mit 25 und mehr Transaktionen/Jahr.

## Mit EverReal verbinden

1. Um einen EverReal-Use-Case zu nutzen, müssen Sie sich gegenüber der **EverReal API** authentifizieren. Hierzu benötigen Sie:
   1. **Benutzername**
   2. **Password**
   3. **Subdomain**:\
      Die Subdomain finden Sie, wenn Sie in Ihrem EverReal Account eingeloggt sind oben in der URL Leiste. Hier wird ein Link mit folgender Anfangsstruktur zu sehen sein: [https://**aareon-connect**.everreal.co/app/](https://sandbox-aareon-connect.everreal.co/app/) Dort wo im Beispiel aareon-connect in fett und kursiv steht finden Sie Ihre Subdomain.
2. Nachdem Sie Aareon Connect Kunde geworden sind, können Sie die verfügbaren **EverReal Integrationen innerhalb Ihres ERP-Systems** auswählen und aktivieren.

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](../use-cases/stammdaten.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

#### Entitäten

| ERP                                                            | EverReal                                   |
| -------------------------------------------------------------- | ------------------------------------------ |
| [Wirtschaftseinheiten](../entitaeten/wirtschaftseinheiten.md)  | Objektgruppen                              |
| [Gebäude](../entitaeten/gebaeude.md)                           | Objekte                                    |
| [Verwaltungseinheiten](../kategorien/eigentuemerverwaltung.md) | Einheiten                                  |
| [Mietverträge](../entitaeten/mietvertraege.md)                 | Vertragsinformationen hängen am Mieter     |
| [Mieter](../entitaeten/mieter.md)                              | Mieter (Typ: Mieter)                       |
| [Eigentümervertrag](../entitaeten/eigentuemervertraege.md)     | Vertragsinformationen hängen am Eigentümer |
| [Eigentümer](../entitaeten/eigentuemer.md)                     | Eigentümer (Typ: Eigentümer)               |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="165">Name</th><th width="290.33333333333326">Beschreibung</th><th>Optionen</th><th data-type="checkbox">UTS</th><th data-type="checkbox">Sigma</th><th data-type="checkbox"></th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Seperator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td><td>false</td><td>false</td><td>false</td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td><td>false</td><td>false</td><td>false</td></tr><tr><td>Wirtschaftseinheiten Nummern</td><td>Es werden nur Daten für die eingetragenen Wirtschaftseinheiten synchronisiert.</td><td></td><td>false</td><td>false</td><td>false</td></tr><tr><td>ERP Gebäude importieren</td><td>Wenn diese Option ausgeschaltet ist, werden keine Wirtschaftseinheit in EverReal erstellt. Stattdessen werden Wirtschaftseinheiten aus dem ERP als Objekte in EverReal erstellt. Die Gebäude-Ebene aus dem ERP fällt somit ganz in EverReal weg.</td><td>Ja / Nein</td><td>false</td><td>false</td><td>false</td></tr><tr><td>Kosten Mapping</td><td>Die jeweiligen Kosten Bezeichnungen aus dem ERP werden zu den folgenden drei Kosten Kategorien aus EverReal zugeordnet:<br>- Kalt Miete<br>- Nebenkosten<br>- Heizungskosten<br><br>Tragen Sie die genutzen Bezeichnungen in die Felder der jeweiligen Kategorien ein</td><td></td><td>false</td><td>false</td><td>false</td></tr><tr><td>Kosten Mapping: Standard Kategorie</td><td>Diese Kategorie wird genutzt, falls Kosten Bezeichnung nicht in obigen Mappings vorhanden ist.<br>Es ist somit die 'Standard Kategorie' für Kosten, falls nicht explizit im Mapping spezifiziert.</td><td><code>Kalt Miete</code>, <code>Nebenkosten</code> , <code>Heizungskosten</code></td><td>false</td><td>false</td><td>false</td></tr></tbody></table>

### 2. Leerstände & Interessenten

#### Übersicht

* [Allgemeine Informationen Leerstände](../entitaeten/leerstaende.md)
* [Allgemeine Informationen Interessenten](../use-cases/interessenten.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=96033489\&fvid=276732562)

| ERP                                           | EverReal             |
| --------------------------------------------- | -------------------- |
| [Leerstand](../entitaeten/leerstaende.md)     | Anzeigen             |
| [Interessent](../entitaeten/interessenten.md) | Interessent / Mieter |

#### Einstellungen

| Name                                 | Beschreibung                                                                                                                                                                                                                        | Optionen         |
| ------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- |
| System für Auswahl von Interessenten | <p>Wenn die Auswahl von Interessenten im ERP geschieht, werden  alle Interessenten von EverReal zum ERP synchronosiert.<br>Wenn die Auswahl in EverReal stattfindet, werden nur die ausgewählten Mieter zum ERP synchronisiert.</p> | `ERP`, `Partner` |

Detaillierte Einstellungen für den Export von Leerstanden werden direkt im ERP vorgenommen.
