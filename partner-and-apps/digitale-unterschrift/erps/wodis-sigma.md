# WODIS Sigma

## Initiale Einrichtung

{% hint style="info" %}
Diese Einrichtung wird aktuell von einem Aareon Berater für Sie vorgenommen.
{% endhint %}

Nachdem Sie die Digitale Unterschrift wie in [#aktivierung-in-aareon-connect](../scrive-technologie-partner.md#aktivierung-in-aareon-connect "mention") beschrieben aktiviert haben muss zuletzt die Verknüpfung zwischen WODIS Sigma und Aareon Connect eingerichtet werden:

1. **TODO**: Beschreiben von Hinterlegen der Locoia Proxy Daten
2. **TODO**: Restlichen Prozess beschreiben

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
