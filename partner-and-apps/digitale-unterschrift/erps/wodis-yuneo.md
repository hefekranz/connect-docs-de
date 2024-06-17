# WODIS Yuneo

## Initiale Einrichtung

### Lizenzen Einlesen

Lesen Sie wie [hier beschrieben](../../../erps/wodis-yuneo.md#aareon-connect-in-wodis-yuneo-aktivieren-lizenzen-einlesen) die aktuellen Lizenzen ein.

### Verknüpfung zwischen WODIS Yuneo und Aareon Connect herstellen

Nachdem Sie die Digitale Unterschrift wie in [#aktivierung-in-aareon-connect](../scrive-technologie-partner.md#aktivierung-in-aareon-connect "mention") beschrieben aktiviert haben muss zuletzt die Verknüpfung zwischen WODIS Yuneo und Aareon Connect eingerichtet werden.

1. Gehen Sie auf **Systemeinrichtung** > **Optionen** > **Optionen Allgemein** > **Digitale Unterschrift**
2. Setzen Sie **Digitale Unterschrift** auf **Konfigurieren**
3. Wählen Sie **Scrive** bei **Technologiepartner** aus
4. Tragen sie den **Benutzernamen**, **Passwort** und **Integrations ID** ein, welche Sie nach der [#aktivierung-in-aareon-connect](../scrive-technologie-partner.md#aktivierung-in-aareon-connect "mention") erhalten haben
5. Unter der Integrations-ID können Sie bei **Vorbelegung Versandreihenfolge** die standard **Reihenfolge** nach Unterzeichner Gruppe (Intern und Extern) bestimmen, in der die Vertragsparteien unterzeichnen sollen.\
   Bei **Versand pro Gruppe** können Sie bestimmen, ob alle Unterzeichner der jeweiligen Gruppe **Gleichzeitig** oder basierend auf der Reihenfolge in der Aktivität unterzeichnen sollen.\
   Diese standard Reihenfolge können Sie, wenn gewünscht, in jedem einzelnem Vorgang überschreiben.
6. Klicken Sie auf **Speichern**

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

### Arbeitsaufträge Einrichten

Nun müssen noch die passenden Arbeitsaufträge angelegt werden:

1. Gehen Sie auf **Systemeinrichtung** > **Organisation und Datenmanagement** > **Planung Arbeitsaufträge**
2. Klicken Sie oben links auf **Neu anlegen**
3. Suchen Sie im **Typ** Feld nach **Digitale Unterschrift - Dokumente versenden**
4. Geben Sie dem Arbeitsauftrag einen Namen
5. Stellen Sie einen Zeitraum ein. Wir empfehlen den Job mehrmals täglich ausführen zu lassen (z.B. alle 2 Stunden)
6. Klicken Sie auf **Speichern**
7. Wiederholen Sie die Schritte 2-6 für den Arbeitsauftrags-Typ **Digitale Unterschrift - Dokumente empfangen**

<figure><img src="../../../.gitbook/assets/image (33) (1).png" alt=""><figcaption></figcaption></figure>

## Einmalige Einrichtung je Dokumentvorlage

Die folgenden Schritte müssen Sie nur einmalig je Dokumentvorlage durchführen. Durch diese Schritte fügen Sie so genannte "Anchor Tags" zu Ihren Dokumentvorlagen hinzu.

Die Anchor Tags werden im Unterzeichnungsvorgang den passenden Unterzeichnern zugeordnet, sodass diese an den von Ihnen vorgesehenen Stellen Unterschreiben oder Felder ausfüllen.

1. Gehen Sie auf **Vorlagenverwaltung** > **Erstellung einer Serienbriefvorlage**
2. Klicken Sie, in der Vorlage, auf **Vorlage bearbeiten**
   1. Somit öffnet sich die Vorlage in Wodis Text
3. Gehen Sie im oberem Menü auf den Reiter **Seriendruck**
4. Klicken Sie im Dokument auf die Stelle, wo sie ein Anchor Tag einfügen wollen
5. Klicken Sie auf den, unter dem oberem Menü, Knopf **Feld erstellen**
6. Konfigurieren Sie das Feld und bestätigen die Konfiguration mit einem Klick auf **Einfügen**
   1. Es stehen folgende Konfigurationsmöglichkeiten zur Verfügung:
      1. Unterzeichner
         1. Intern _- Unternehmensinternem (z.B. Sachbearbeiter_
         2. Extern _- Externe Person (z.B. Mieter)_
      2. Unterzeichner Nr. _- Zuordnung der Unterzeichner innerhalb der jeweiligen Internen bzw. Externen Unterzeichner_
      3. Feldart
         1. Unterschrift
         2. Unterschriftsdatum _- Das aktuelle Datum_
         3. Datum
         4. Name
         5. Checkbox
         6. Text
         7. Email
         8. Initialen _- Die jeweils ersten Buchstaben des Vor- und Nachnamens (z.B. bei Erika Mustermann: EM)_
      4. Feld Nr. - _Zuordnung der Felder innerhalb der jeweiligen Feldarten_
      5. Feldeigenschaft
         1. Pflicht _- Das Feld muss zwingend ausgefüllt werden_
         2. Optional _- Das Feld kann ausgefüllt werden_
7. Nachdem Sie alle Anchor Tags eingefügt haben, gelangen Sie zurück in die Vorlagenverwaltung mit Klick auf **Datei**
8. Scrollen Sie zum Bereich **Archivierung**
9. Klicken Sie auf **Archivieren**
   1. _Hintergrund_: Ohne Archivierung des Dokuments ist die Digitale Unterschrift nicht möglich
10. Klicken Sie oben rechts auf **Speichern**

## Prozess je Dokument

### Einrichten und Versenden von Dokumenten

Nachdem Sie die [#einmalige-einrichtung-je-dokumentvorlage](wodis-yuneo.md#einmalige-einrichtung-je-dokumentvorlage "mention") vorgenommen haben, können Sie Dokumente ganz einfach, als Teil des regulären Schriftverkehr-Prozess, digital unterschreiben lassen.

Bei dem Schriftverkehr Erstellungs-Prozess müssen Sie dafür folgende Dinge beachten:

1. Sie können nur Dokumentvorlagen verwenden, welche Sie wie in [#einmalige-einrichtung-je-dokumentvorlage](wodis-yuneo.md#einmalige-einrichtung-je-dokumentvorlage "mention") beschrieben eingerichtet haben
2. Bei der Schriftverkehrs-Aktivität in der Sektion **Aktivität - Allgemein** folgende Einstellungen vornehmen:
   1. Systemtyp: Aufgabe
   2. Aktivitätstyp: Digital Unterschreiben
   3.  Die weiteren Felder können Sie individuell ausfüllen

       <figure><img src="../../../.gitbook/assets/image (7).png" alt="" width="563"><figcaption></figcaption></figure>
3. Fügen Sie bei der Sektion **Bearbeitet von** mindestens einen Benutzer hinzu
4. In der Sektion **Digitale Signatur** können Sie alle Unterzeichner hinzufügen
   1. Bei **Intern** wählen Sie einen oder mehrere Yuneo Benutzer (Unternehmensinterne Person) aus
   2. Bei **Extern** wählen Sie einen oder mehrere Kontakt(e) aus (externe Personen)
5. In dem Feld **Reihenfolge** können Sie auswählen, ob Sie Ihre Auswahl aus den Standardeinstellungen übernehmen wollen oder eine andere Reihenfolge bestimmen.

<figure><img src="../../../.gitbook/assets/MicrosoftTeams-image.png" alt=""><figcaption></figcaption></figure>

#### Vor-Ort-Unterschrift

Um die Vor-Ort-Unterschrift zu nutzen, müssen diese drei Schritte befolgt werden:

1. Klicken Sie bei **Vor-Ort-Unterschrift** auf **Ermöglichen**
2. Tragen Sie eine E-Mail Adresse in dem Feld **E-Mail Adresse für Vor-Ort-Unterschrift** ein
3. Klicken Sie in die Checkbox **Vor Ort unterschreiben** für die Unterzeichner die vor Ort unterschreiben sollen

<figure><img src="../../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

### Empfangen und Sichten von unterschriebenen Dokumenten

Yuneo holt sich regelmäßig (Standard: alle 30 Minuten) den aktuellen Stand aller Dokumente.\
Die Einstellungen dafür sind wie in [#initiale-einrichtung](wodis-yuneo.md#initiale-einrichtung "mention") beschrieben hinterlegt.

1. Im Yuneo **Cockpit** können Sie den Status aller Digitalen Unterschrifts-Dokumente einsehen
2. Durch Klick auf einer dort angezeigten Aktivität sehen Sie die Details der Aktivität, das unterschriebene Dokument, das Unterschriftszertifikat und weitere Informationen
