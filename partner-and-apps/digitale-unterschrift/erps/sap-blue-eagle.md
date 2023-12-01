# SAP Blue Eagle

## Initiale Einrichtung

{% hint style="success" %}
Diese Schritte werden von einem Aareon Berater für Sie durchgeführt.
{% endhint %}

Diese Schritte müssen nur einmalig im ERP System vorgenommen werden, damit die Digitale Unterschrift genutzt werden kann

1.  **Vorbelegung der Zuordnung**

    <figure><img src="../../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>

    1. Legen Sie den Vorgang bei erfolglosem Signaturprozess durch den Berater fest. (Dient dazu, zu bestimmen was passiert, wenn eine Vertragspartei die Signatur ablehnt
    2. Stellen Sie unter der Spalte Code ein, welcher Vorgang aufgehen soll, damit der Sacharbeiter weiß, dass der Vertragspartner die Unterschrift abgelehnt hat.
2.  **Einstellung der Geschäftspartner nach Rollen**

    <figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

    1. Stellen Sie die Geschäftspartner nach Rollen ein (Berater)&#x20;
    2. Richten Sie die ABAB-Programme zur Ermittlung der Geschäftspartner ein. (in der Tabelle unter Haupt)&#x20;
    3. Ordnen Sie die nötigen Vorgänge den Geschäftspartnern zu. Prozess --> Versand der Dokumente dem Geschäftspartner zuordnen, der sie bekommen soll.
3.  **Einrichten der 2-Faktor-Authentifzierung**

    <figure><img src="../../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

    1. Tragen Sie in der Tabelle den Buchungskreis, die Kommunikation und den Telefontyp ein
4.  **Status der Aktionen/ Maßnahmen ignorieren**

    <figure><img src="../../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

    1. Klicken Sie dann auf den Ordner **Status der Aktionen/ Maßnahmen ignorieren**
    2. Klicken Sie auf Ignorieren für jeden Buchungskreis

## Einmalige Einrichtung je Dokumentenvorlage

Die folgenden Schritte müssen Sie nur einmalig je Dokumentenvorlage durchführen. Durch diese Schritte fügen Sie so genannte "Anchor Tags" zu Ihren Dokumentvorlagen hinzu.

Die Anchor Tags werden im Unterzeichnungsvorgang den passenden Unterzeichnern zugeordnet, sodass diese an den von Ihnen vorgesehenen Stellen Unterschreiben oder Felder ausfüllen.

<figure><img src="../../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

1. Sammeln Sie Ihre Dokumente in Dynamic Forms
2. Allgemein > Customizing > Dynamics Forms > Dynamic Forms bearbeiten
3. Wählen Sie ein Dokument aus > Textbausteine

## Prozess je Dokument

Einrichten und Versenden von Dokumenten

<figure><img src="../../../.gitbook/assets/Group 1 (2).png" alt=""><figcaption></figcaption></figure>

1. Klicken Sie auf **Kundenkontakte** und dann in dem sich öffnende Drop Down Feld auf **"Mietsache"**

### 1.1 Anlage neuer KKM Vorgang &#x20;

1.  Klicken Sie auf **Vorgang anlegen** und wählen Sie die Art im Drop Down Feld aus. (Der Vorgang kann auch automatisiert bei Vertragsanlage erstellt werden (kostenpflichtiges Addon -> Beraterlösung)



    <figure><img src="../../../.gitbook/assets/Vorgang anlegen Mietsache.png" alt=""><figcaption></figcaption></figure>
2. Wählen Sie über **Vorgangsgruppe** den **digitalen Mietvertrag** aus

<figure><img src="../../../.gitbook/assets/Group 10.png" alt=""><figcaption></figcaption></figure>

1. Wählen Sie in dem sich öffnenden Fenster den **digitalen Mietvertrag** aus und klicken sie auf Ausgang
2. Speichern Sie den Vorgang
3.  Klicken Sie auf **"Aktion/Maßnahmen/Folgevorgänge"**



### **1.2 Dokument auswählen**

1. Klicken Sie auf **"Erstellen Korrespondenz digitaler Mietvertrag"**

<figure><img src="../../../.gitbook/assets/Erstellen Korrespondenz digiataler Mietvertrag.png" alt=""><figcaption></figcaption></figure>

### 1.3 Dokumentenauswahl und Archivierung

<figure><img src="../../../.gitbook/assets/Ablagemodus Drop Down Feld.png" alt=""><figcaption></figcaption></figure>

1. Wählen Sie ihre Dokumente aus (In diesem Beispiel Online Mietvertrag)
2. Stellen Sie den Ablagemodus im Drop Down Feld wie oben rechts auf dem Screenshot zu erkennen ist auf **2 Nur Ablegen** ( kann auch voreingestellt werden)
3. Archivieren Sie das Dokument durch den Klick auf Drucken
4. Gehen Sie dann zurück

### **1.4 Versand Dokumente**

<figure><img src="../../../.gitbook/assets/Versand Dokumente.png" alt=""><figcaption></figcaption></figure>

1. Klicken Sie auf den Button Rechts neben Versand Dokumente
2. Klicken Sie dann auf **alle senden** und bestätigen Sie durch den Klick auf **"Ja"** im Pop-up

### 1.5 Versand erfolgreich

<figure><img src="../../../.gitbook/assets/Versand erfolgreich.png" alt=""><figcaption></figcaption></figure>

1. Das Dokument wurde erfolgreich versendet und Sie erhalten, wie auf dem Screenshot zu erkennen ist, einfache Zweifache- Bestätigung.
2. Alle nötigen Unterzeichner bekommen das Dokumenten nun in DocuSign zu Verfügung gestellt und können ihre Signatur darunter setzten- Vertrag wird abgeschlossen.



### 2. Empfangen und Sichten von unterschriebenen Dokumenten

<figure><img src="../../../.gitbook/assets/Group 20.png" alt=""><figcaption></figcaption></figure>

1. Statusaktualisierung erfolgt automatisiert, optional manuell
2. Ihr Status Text ändert sich zu: **"Wartet auf Unterzeichnung"**
3. Sie haben die Möglichkeit den Status zu aktualisieren  durch den klick auf: **" Status abfragen"**
4. Sie haben eine Möglichkeit eine Erinnerung zusenden durch den Klick auf: **"Erinnerung senden"**

### 2.1 Nach Ausgang des Mietvertrags

<figure><img src="../../../.gitbook/assets/Group 22 (1).png" alt=""><figcaption></figcaption></figure>

1. Anhand des **grünen Rechtecks** sehen Sie, dass der Ausgang des digitalen Mietvertrags abgeschlossen ist.
2. Anhand der **Vorgangsnummer** sehen Sie, dass der rücklaufende digitale Mietvertrag nun die entsprechenden Anlagen der Mietverträge und des jeweiligen Zertifikats hat.
3. Klicken Sie auf **Anlagen,** um den Mietvertrag und Zertifikat einzusehen
4. Klicken Sie auf **"Online Mietvertrag"** zur Durchsicht des abgeschlossenen Mietvertrags.
5. Klicken Sie auf **Zertifikat** zur Durchsicht
