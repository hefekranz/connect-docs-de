---
description: >-
  Optimieren der Immobilienkommunikation durch einfach integrierbare,
  mehrsprachige K.I.-Chat- und Voicebots von Bots4You, datenschutzkonform und
  benutzerfreundlich.
---

# Bots4You

## Übersicht

* **Kategorien**: [Mieterkommunikation](../kategorien/mieterkommunikation.md), [Reporting](../kategorien/reporting.md), [Dokumentenmanagement](../kategorien/dokumentenmanagement.md)
* **Use Cases**: [Stammdaten](../use-cases/stammdaten.md), [Tickets](../use-cases/tickets.md)
* **Marketplace**: [Bots4You](https://marketplace.aareon.com/de/listings/bots4you)

## Beschreibung

Bots4You bietet K.I.-gestützte Chatbots und Voicebots, die speziell für den Einsatz im Immobilienmanagement entwickelt wurden. Diese Technologie zielt darauf ab, die Kommunikation zwischen Immobilienunternehmen und ihren Kunden oder Mitarbeitern zu verbessern. Die Plattform von Bots4You, die keine Programmierkenntnisse erfordert, ermöglicht es Nutzern, K.I.-Lösungen einfach zu implementieren. Die Bots sind mehrsprachig, anpassbar und können auf verschiedenen Plattformen wie Websites oder als Telefon-Assistenten eingesetzt werden, wobei sie stets datenschutzkonforme Richtlinien befolgen. Durch die Integration mit internen Systemen der Unternehmen können die Bots effektiv Informationen austauschen, wodurch Prozesse optimiert und die Kundenzufriedenheit potenziell gesteigert wird. Bots4You bietet somit eine Vielzahl von Anwendungsmöglichkeiten für die interne und externe Kommunikation im Immobiliensektor. Bei weiteren Fragen zur Anbindung melden Sie sich direkt bei Bots4You.



## Server und Hosting

Die [KI-basierte virtuelle Assistentin Neela](https://einfach.aareon.de/CRM-Portal-App.727021.html), die mit dem Aareon CRM. erworben wird, ist im Aareon-Rechenzentrum gehostet (die Server betrieben).

Andere Produkte wie der VoiceBot oder Omni-Channel von Bots4You werden primär in der Telekom Cloud in Deutschland, aber auch bei Stack IT gehostet.

## Mit Bots4You verbinden

1. Um einen Bots4You-Use-Case zu nutzen benötigen Sie zur Aktivierung die **Bots4You API Zugangsdaten**. Diese sind folgendermaßen:
   1. **Username**
   2. **Passwort**

## Use Cases

### 1. Stammdaten

#### Übersicht

* [Allgemeine Informationen](https://connect-docs-de.locoia.com/use-cases/stammdaten)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

Die Stammdaten werden nur vom ERP zu Bots4You übertragen.

#### Entitäten

| ERP                                                                         | Bots4You |
| --------------------------------------------------------------------------- | -------- |
| [Mieter](https://connect-docs-de.locoia.com/entitaeten/mieter)              | Mieter   |
| [Mietverträge](https://connect-docs-de.locoia.com/entitaeten/mietvertraege) | Mieter   |

#### Einstellungen

Im Zuge der Aktivierung des Stammdaten Use Cases, können Sie folgende Einstellungen nutzen:

<table><thead><tr><th width="165">Name</th><th width="450.33333333333326">Beschreibung</th><th>Optionen</th></tr></thead><tbody><tr><td>Separator für zusammengesetzte IDs</td><td>Dieser Separator wird genutzt um die IDs in dem Partner System aus den ERP Nummern zusammenzusetzen, sodass die IDs eindeutig sind.</td><td><code>-</code>, <code>_</code>, <code>.</code>, <code>/</code>, <code>|</code></td></tr><tr><td>Mandanten Nummern</td><td>Es werden nur Daten für die eingetragenen Mandanten synchronisiert.</td><td></td></tr></tbody></table>

### 2. Tickets

#### Übersicht

* [Allgemeine Informationen](../use-cases/tickets.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

Die Ticket Kategorien werden nur vom ERP zu Bots4You übertragen.

Tickets die in Bots4You erstellt werden, werden an das ERP übertragen und der Status dieser Tickets wird zurück vom ERP an Bots4You übertragen.\
Tickets die im ERP erstellt wurden, werden nicht an Bots4You übertragen.

#### Entitäten

| ERP               | Bots4You          |
| ----------------- | ----------------- |
| Tickets           | Tickets           |
| Ticket Kategorien | Ticket Kategorien |

## Sonstiges

### Voicebot: Fragen und Schritte zur Vorbereitung

* Nennen Sie uns bitte einen Kontakt des Anbieters Ihrer Telefonanlage und den Namen der Anbieterfirma?
* Wie lassen sie heute Anrufer sich authentifizieren?
* In welche Sprachen lassen Sie rechtsverbindliche Aussagen am Telefon zu?
* Wer reguliert Schäden - intern vs. extern?
* Sind Sie selbst als Verwalter aktiv oder haben Sie Unterverwalter?



### FAQs



**Wo stehen die Server?**\
Europa, DSGVO-Konform.\


**Wie sind die Authentifizierungsmöglichkeiten?**

Klassische Authentifizierung über Mietvertragsnummer sowie andere gewünschte Parameter (individuell einstellbar). \


**Wie kann ich eine Telefonanlage für den VoiceBot verbinden?**

Es gibt folgende Möglichkeiten:

1. Weiterleitung einer Rufnummer and die Rufnummer des Bots. Diese wird von Bots4You eingerichtet.
2. Man kann zu verschiedenen Telefonzeiten verschiedene Aktionen durchführen, wobei die  Möglichkeiten von der Telefonanlage abhängt.

**Welche Telefonnummern kann man hinter den VoiceBot schalten?**

1. Mit SIP Trunk kann man die Nummer einer Telefonanlage direkt nutzen.
2. Ansonsten wird eine Nummer von Bots4You vorgegeben auf diese üblicherweise weitergeleitet.

**EmailBot: Wie kann dieser mit Outlook verknüpft werden?**

Die Outlook Microsoft Azure App muss verwenden werden.

Neben dem Email-Bot kann man dann zusätzlich selbst schreiben auf z.B. einem Sammelpostfach. Allerdings wird Bots4You die einkommenden E-Mails auslesen und darauf direkt reagieren.



**Erfolgt eine Aufzeichnung der Telefonate oder wird nur transkribiert?**\
Es wird im Standard nur transkribiert.



**Kann ein Telefonanlage schon vorab Anrufer authentifizieren und diese Identifizierung weitergeben an den Voicebot?**

Ja, der einfachste Weg ist, wenn die Telefonanlage an den Voicebot anruft und dabei in Abhängigkeit des Authentifizierungsstatus die Rufnummer in der Weiterleitung mitschickt, wenn der Anrufer nicht authentifiziert ist und die Mietvertragsnummer, wenn der Anrufer authentifiziert ist.\
\


**Verlängert sich die Dauer eines Telefonast des Voicebots, wenn dieser den Mieter identifizieren soll?**\
Ja, die Identifizierung kostet einige Sekunden.



**Angenommen in der Telefonwarteschleife befinden sich 5 Wartende: Kann der Voicebot alle Mietenden gleichzeitig bedienen?**\
&#x20;Ja, es können gleichzeitig verschiedne Anrufer weitergeleitet werden.



**Was passiert, wenn der Voicebot ein Anliegen nicht versteht?**\
Das kann im Dialog-Builder definiert werden. Z.B. kann eine Rückrufbitte eingestellt werden.



**Müssen Audio-Dateien gelöscht werden?**\
Nein, es werden keine Audio-Dateien aufgezeichnet. Daher muss nichts gelöscht werden.



**Kann die anrufende Telefonnummer im ERP aktualisiert werden, wenn unter der legitimierten Vertragsnummer noch eine alte Telefonnummer hinterlegt ist?**\
Nein, nicht im Standard. Das wäre eine zusätzlich zu beauftragende Zusatzfunktion.
