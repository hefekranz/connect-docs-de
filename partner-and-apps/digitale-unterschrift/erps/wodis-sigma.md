# WODIS Sigma

## Initiale Einrichtung

### Lizenzen Einlesen

Lesen Sie wie [hier beschrieben](../../../#wodis-sigma) die aktuellen Lizenzen ein.

### Verknüpfung zwischen WODIS Sigma und Aareon Connect herstellen

Nachdem Sie die Digitale Unterschrift wie in [#aktivierung-in-aareon-connect](../scrive-technologie-partner.md#aktivierung-in-aareon-connect "mention") beschrieben aktiviert haben muss zuletzt die Verknüpfung zwischen WODIS Sigma und Aareon Connect eingerichtet werden.

1. Gehen Sie auf **Zentrale Funktionen** > **Aktivitätenmanagement** > **Stammdaten** > **Aktivitätenmanagement Einstellungen**
2.  Tragen Sie für das Feld **Digitale Signatur Logins** den Wert **Scrive** in die Spalte **Benutzerwert** ein\


    <figure><img src="../../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>
3. Somit erscheinen die benötigten Felder
4. Tragen sie die Daten welche Sie nach der [#aktivierung-in-aareon-connect](../scrive-technologie-partner.md#aktivierung-in-aareon-connect "mention") erhalten haben in die entsprechenden Felder ein:
   1. **Benutzernamen** in das Feld **Scrive: Digitale Signatur User**
   2. das **Passwort** in das Feld **Scrive: Digitale Signatur Password**
   3. die **URL** in das Feld **Scrive: Digitale Signatur Url**
   4. und die **Authentication URL** in das Feld **Scrive: Digitale Signatur Auth Url**

{% hint style="info" %}
Die Felder **Scrive: Digitale Signatur Fingerprint** und **Scrive: Digitale Signatur Tenant Id** können Sie leer lassen.
{% endhint %}

### Arbeitsaufträge Einrichten

{% hint style="warning" %}
Dokumentation folgt in Kürze
{% endhint %}

## Vorbereitung Ihrer Dokumente

Für die Digitale Unterschrift nutzen Sie wie gewohnt den Schriftverkehr in WODIS Sigma ([weitere Informationen](https://www.aareon.de/Support\_und\_Wissen/Dossier\_Schriftverkehr\_mit\_Wodis\_Sigma.212684.html) \[Verlinkung auf Aareon Support und Beratung, Zugang nur mit Login möglich]).

Verschiedenste Anchor Tags, die im Unterzeichnungsvorgang den passenden Unterzeichnern zugeordnet werden, sodass diese an den von Ihnen vorgesehenen Stellen Unterschreiben oder Felder ausfüllen, können hinzugefügt werden.

Dabei gibt es folgende Möglichkeiten:

1. <mark style="background-color:blue;">Unterzeichner</mark>
   1. Intern _- Unternehmensinternem (z.B. Sachbearbeiter_
   2. Extern _- Externe Person (z.B. Mieter)_
2. <mark style="background-color:purple;">Unterzeichner Nummer</mark> - _Zuordnung der Unterzeichner innerhalb der jeweiligen Internen bzw. Externen Unterzeichner_
3. <mark style="background-color:orange;">Feldart</mark>
   1. Unterschrift
   2. Unterschriftsdatum _- Das aktuelle Datum_
   3. Datum
   4. Name
   5. Checkbox
   6. Text
   7. Email
   8. Initialen _- Die jeweils ersten Buchstaben des Vor- und Nachnamens (z.B. bei Erika Mustermann: EM)_
4. <mark style="background-color:green;">Feld Nummer</mark> _- Zuordnung der Felder innerhalb der jeweiligen Feldarten_
5. <mark style="background-color:red;">Feldeigenschaft</mark>
   1. \* _- Das Feld muss zwingend ausgefüllt werden_
   2. ? _- Das Feld kann ausgefüllt werden_

Dies muss in dem folgendem Syntax zusammengesetzt werden (die einzelnen Bestandsteile sind farblich markiert), hier z.B. für das erste Unterschriftsfeld für den ersten internen Unterzeichner:

DU.<mark style="background-color:blue;">Intern</mark>.<mark style="background-color:purple;">01</mark>.<mark style="background-color:orange;">Unterschrift</mark>.<mark style="background-color:green;">01</mark><mark style="background-color:red;">\*</mark>

Das dritte optionale E-Mail Feld für den zweiten externen Unterzeichner muss entsprechend wie folgt in dem Dokument hinterlegt werden:

DU.<mark style="background-color:blue;">Extern</mark>.<mark style="background-color:purple;">02</mark>.<mark style="background-color:orange;">Email</mark>.<mark style="background-color:green;">03</mark><mark style="background-color:red;">?</mark>

{% hint style="warning" %}
Der Syntax muss genau befolgt werden, damit die Anchor Tags ausgelesen werden können.

Alle Anchor Tags müssen mit **DU.** starten.
{% endhint %}

Die Anchor Tags sollten mit weißer Schrift in den Dokumenten hinterlegt werden, damit diese für die Unterzeichner nicht sichtbar sind, aber vom ERP und Scrive ausgelesen werden können.

## Prozess je Dokument

### Einrichten und Versenden von Dokumenten

1. Mietvertragsauswahl
   1. **Modul Mietvertrag** auswählen und dann in der Suchleiste den betroffenen Mietvertrag eingeben
2. Archivieren des Vertrags
   1. klicken Sie auf oben rechts auf **Dokumente** und dann **Archivieren**
   2.  Dokumententyp **Mietvertrag** auswählen:\


       <figure><img src="../../../.gitbook/assets/Group 25.png" alt=""><figcaption></figcaption></figure>
   3. Auf den Ordner **Dateisyteme** oben in der Leiste klicken und dann Mietvertrag auswählen und dann oben links in der Leiste auf **Archivieren** drücken
3. Neue Anfrage erstellen
   1. Klicken Sie oben rechts in der Taskleiste auf **Daten neu** (Symbol mit dem grünen + Zeichen)
   2. Passen Sie die Unterzeichner an
   3. Geben Sie: **"$" + "Name"** ein für die Schnellauswahl des internen Unterzeichners
   4. In dem Feld **neue Aktivität zum Mietvertrag** geben Sie den Betreff für die Anfrage der digitalen Signatur an
   5. Dann klicken Sie eine Zeile drunter auf **Anhang** du suchen durch die Nummer das Vertragsdokument aus
   6. Wählen Sie das Dokument aus, durch den Klick auf **Übernehmen**.
4. Hinzufügen von Anchor Tags
   1. Klicken Sie auf **Digitale Signatur** rechts unter **Anhang** und dann auf das Kästchen **Signatur**
      1. Zum Hinzufügen der Unterzeichner klicken Sie auf **Hinzufügen** und wählen Sie dann den Unterzeichner aus
      2. Ordnen Sie die Unterzeichnern den im Dokument definierten Anchor Tags zu
   2. Den selben Prozess können Sie dann für die anderen Anchor Tags Feldtypen folgen
5. Durchführen der Jobplanung\

   1. Wählen Sie das Modul **Job Planung** aus
   2. Gehen Sie oben in der Taskleiste auf **die Lupe** und suchen Sie den Jobplanungseintrag **(DS Anchortags)** in der Tabelle
   3. Geben Sie den Auftrag bei dem Kästchen **Status** frei.
   4. Legen Sie den Zeitpunkt der Ausführung fest
   5. Klicken Sie dann auf **Speichern**
   6. Somit wird das Dokument zum geplanten Zeitpunkt per Scrive an die angegebene E-Mail-Adressen versendet
6.

    <figure><img src="../../../.gitbook/assets/Group 26.png" alt=""><figcaption></figcaption></figure>

### Empfangen und Sichten von unterschriebenen Dokumenten

1. Durchführung der Job Planung zum Einholen der Vertragsdaten
   1. Wählen Sie das Modul **Job Planung** aus
   2. Suchen Sie den Jobplanungseintrag **DS Anchortags** abholen
   3. Setzten Sie den **Status** auf Freigeben
   4. Legen Sie den Zeitpunkt der Ausführung fest
   5. Klicken Sie dann auf **Speichern**
2. Durchsicht des signierten Dokuments
   1. Klicken Sie rechts neben dem Reiter Aufgaben **auf Anhang**
   2. Klicken Sie auf das zutreffende Dokument
   3. Klicken Sie dann oben in der Taskleiste **auf Anhänge**
   4. Wählen Sie das Dokument per Klick aus

## Erfolgskontrolle der Durchführung des Jobs

Falls Sie ungewöhnlich lange auf ein Dokument warten oder eine Fehlermeldung in der Job Durchführung erhalten haben, können Sie wie folgt Erfolgskontrollen durchführen.

### Erfolgskontrolle im Job

1. Klicken Sie auf Meldung: **(Uhrzeit) Der Job (…) wurde erfolgreich beendet.**
2. Klicken Sie auf **Report anzeigen**
3. Fehlerkontrolle, wenn bei Ihnen steht kein Fehler wurde das Dokument erfolgreich gesendet.
4. Kontrollieren Sie, ob der Job erfolgreich durchgeführt worden ist in dem Sie auf “der Job wurde erfolgreich beendet” klicken und dann auf Report anzeigen
5. Kontrollieren Sie die Anzahl der Signierten Dokumente und ob der Signaturprozess erfolgreich durchgeführt worden ist. Dies ist der Fall, wenn in den Meldungen der Satz: (Fehler: Kein Fehler steht)

### Erfolgskontrolle im Mietvertrag

1. Wählen Sie das Modul Mietvertrag aus
2. Wählen Sie den passenden Mietvertrag aus
3. Klicken Sie oben rechts in der Taskleiste auf Liste
4. Klicken Sie rechts neben dem Mietvertrag auf **Aktivitätenmanagement**
5. Wählen Sie die zutreffende Aktivität aus und klicken SIe auf **den Eintrag**
6. Klicken Sie in dann oben links auf **Aufgabe**
7. Kontrollieren Sie, ob der Signaturprozess erfolgreich durchgeführt worden ist
