---
description: >-
  Yarowa: Vereinfachen Sie Auftrags- und Dienstleistermanagement in der
  Immobilienbranche mit einer benutzerfreundlichen SaaS-Lösung
---

# Yarowa

## Übersicht

* **Kategorien**: [Handwerkerportal & Auftragsmanagement](../kategorien/handwerkerportal-and-auftragsmanagement.md)
* **Use Cases**:&#x20;
* **Marketplace**: [Yarowa](https://marketplace.aareon.com/de/listings/yarowa)

## Beschreibung

Yarowa ist eine SaaS-Lösung, die speziell für Immobilienunternehmen entwickelt wurde, um das Dienstleister- und Auftragsmanagement zu digitalisieren und zu professionalisieren. Die Plattform ermöglicht Immobilienunternehmen, Dienstleister aus ihrem eigenen Netzwerk oder dem von Yarowa basierend auf verschiedenen Kriterien auszuwählen. Sie können Angebote anfordern, vergleichen und Aufträge für Reparaturen und Instandhaltungen vergeben sowie deren Ausführung überwachen. Yarowa erleichtert auch die Prüfung und Freigabe von Rechnungen und bietet eine Plattform, die hohe Sicherheitsstandards erfüllt. Sie ermöglicht den direkten Einbezug von Eigentümern, Asset Managern, Mietern und Dienstleistern, wodurch alle Beteiligten stets über den aktuellen Stand und den Fortschritt der Arbeiten informiert sind.

## Mit Yarowa verbinden

1. Um einen Yarowa-Use-Case zu nutzen benötigen Sie zur Aktivierung die **Yarowa API Zugansdaten**. Diese erhalten Sie folgendermaßen:
   1. Melden Sie sich mit Ihren Zugangsdaten (Benutzername und Passwort) bei Yarowa an.
   2. Fügen Sie nun '../dashboard/systemmanagement' an die Basis-URL in der obigen Adressleiste an
   3. Aktivieren Sie die folgenden Optionen:
      1. **Systemintegration aktivieren**
      2. **'Fetch Case Data' aktivieren**
      3. **'Status Update Events' aktivieren**
      4. **Filtern von externen Services aktivieren**
   4.  Klicken Sie auf **Speichern**:

       <figure><img src="../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>
   5. Fügen Sie nun '../dashboard/integrationmanagement' an die Basis-URL in der obigen Adressleiste an
   6.  Klicken Sie auf **Integration hinzufügen**:

       <figure><img src="../.gitbook/assets/image (31).png" alt="" width="288"><figcaption></figcaption></figure>
   7.  Wählen Sie auf der erscheinenden Seite im Dropdown-Feld **Integration Hub Support** **Standard PushnPull PropertyCaseData Gateway Appenzell** wenn sie auf der Testumgebung sind und **Standard**

       **PushnPull PropertyCaseData Gateway Production** wenn sie auf der Produktivumgebung sind aus.
   8.  Wählen Sie den **Integration Mode** **JWT Bearer** aus und klicken Sie auf **Save & Enable**. This will create OAuth2.0

       Dadurch werden OAuth2.0-basierte Client-Anmeldedaten erstellt, die für den Zugriff auf Yarowa-APIs verwendet werden können:

       <figure><img src="../.gitbook/assets/image (39).png" alt="" width="563"><figcaption></figcaption></figure>
2. Nachdem Sie Aareon Connect Kunde geworden sind, können Sie die verfügbaren **Yarowa Integrationen innerhalb Ihres ERP-Systems** auswählen und aktivieren.

## Use Cases

### 1. Stammdaten - In Bearbeitung

#### Übersicht

* [Allgemeine Informationen](yarowa.md#stammdaten)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=1213044489\&fvid=23969279)

### 2. Tickets - In Bearbeitung

#### Übersicht

* [Allgemeine Informationen](../use-cases/tickets.md)
* [Feld Mapping](https://docs.google.com/spreadsheets/d/1b5iCRsnGxBGTXNzHzaNm0SlfRoIpbRofghzS-7HwbVc/edit#gid=388591826\&fvid=1169857418)
