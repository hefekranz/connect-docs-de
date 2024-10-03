# Wodis Yuneo

## Aareon Connect in Wodis Yuneo aktivieren

### 1. Lizenzen Einlesen

Nachdem Sie den Aareon Connect Vertrag unterschrieben haben muss die Lizenz noch in Wodis Yuneo eingespielt werden werden:

1. Gehen Sie auf **Systemeinrichtung** > **Organisation und Datenmanagement** > **Lizenzen**
2.  Klicken Sie im Kopf-Menü auf **Mehr** > **Lizenzen vom Server importieren**\


    <figure><img src="../.gitbook/assets/image (31) (1).png" alt=""><figcaption></figcaption></figure>
3. Bestätigen Sie den eingeblendeten Dialog mit **Importieren**

### 2. Aareon Connect öffnen

Um Aareon Connect in Wodis Yuneo zu öffnen und somit Integrationen zu aktivieren müssen Sie auf **Fachliche** **Einrichtung** > **Integrationen** > **Aareon Connect** gehen oder alternativ nach **Aareon Connect** in **YuSearch** suchen:

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Somit öffnen sich Aareon Connect direkt in Wodis Yuneo:

<figure><img src="../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

## Use Cases

### Leerstände und Interessenten

#### Besonderheiten

Die Use Cases [Leerstände](../use-cases/leerstaende.md) und [Interessenten](../use-cases/interessenten.md) werden bei den Wodis ERPs nicht über eine klassische API Schnittstelle abgedeckt, sondern über die, in die ERPs eingebaute, Immoblue Funktion.

Dies hat den Vorteil, dass Sie das Mapping zwischen ERP und Partner Lösung ganz individuell bestimmen können.

Für das Mapping wird sich der Partner an Sie mit einer Mapping Tabelle wenden, welche dann an die Wodis Beratung weitergegeben wird, welche dieses Mapping entsprechend der Tabelle in Ihrem ERP vornehmen.

Entsprechend dauert der Go-Live Prozess in der Regel etwas länger als bei anderen Use Cases.

{% hint style="warning" %}
Das Trennzeichen der Objektnr. ist bei Wodis Yuneo immer `/`. Bei Wodis Sigma ist dieses frei konfigurierbar.

Je nach Partner gibt es ggf. bestimmte Vorschriften für das Trennzeichen.
{% endhint %}

### Dokumente

Im Zuge der Aktivierung des Dokumenten Use Cases, müssen Sie folgende Einstellungen ausfüllen:

| Name                      | Beschreibung                                                             | Optionen                                                                            |
| ------------------------- | ------------------------------------------------------------------------ | ----------------------------------------------------------------------------------- |
| Mieter Suchkategorien     | Suchkategorien der Archive, die dem Mieter zugeordnet werden sollen      | <p>z.B. :</p><p>„Mieter Dokumente“,</p><p>„Mieter-Freigabe“,</p><p>usw.</p>         |
| Eigentümer Suchkategorien | Suchkategorien der Archive, die den Eigentümern zugeordnet werden sollen | <p>z.B.:</p><p>„Eigentümer Dokumente“,</p><p>„Eigentümmer Freigabe“,</p><p>usw.</p> |
| Schlagwort-Filter         | Schlagwörter/Begriffe die in dem Feld "Bemerkung" enthalten sind         |                                                                                     |

Nutzen Sie zur Übertragung bitte dieses [Formular](https://ivlv.me/OzjIv).

#### Archive

Bei der Bereitstellung von Dokumenten in einer Mieter- oder Eigentümer-App muss definiert werden, aus welchen Archiven Dokumente veröffentlicht werden, damit der Mieter oder Eigentümer keine Dokumente erhält, die nur für den internen Gebrauch vorgesehen waren. Bitte übergeben Sie uns eine Liste der **Suchkategorien**, welche in den zu übertragenden Archiven hinterlegt sind, aus denen wir die Dokumente veröffentlichen sollen.

Die vorhandenen Archive finden Sie in Yuneo, im kompakt Manager und im kompakt Client.

**1. Yuneo**

In der YuSearch „Archiv“ eingeben.

<figure><img src="../.gitbook/assets/Yuneo Archive.png" alt=""><figcaption></figcaption></figure>

**2.Kompakt Manager- hier haben nur Admins Zugang**&#x20;

<figure><img src="../.gitbook/assets/kompact Manager.png" alt=""><figcaption></figcaption></figure>

**Archive**

Im Menüband oben unter Archive werden die Einträge angezeigt

<figure><img src="../.gitbook/assets/kompact Archive Manager (1).png" alt=""><figcaption></figcaption></figure>

&#x20;

**3. Kompakt Client**

Öffnen Sie den **Kompakt Client**

<figure><img src="../.gitbook/assets/kompact client.png" alt=""><figcaption></figcaption></figure>

**Archive**

Im Register Recherche oder Archivierung werden die Archive in den Suchkategorien oder auch in der Mitte unter dem Suchfeld Archiv angezeigt. Hier ein Demo-Archiv. Die Namen stimmen nicht mit Ihren überein.

<figure><img src="../.gitbook/assets/kompact client Achive.png" alt=""><figcaption></figcaption></figure>
