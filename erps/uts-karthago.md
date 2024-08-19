# UTS KARTHAGO

## Schnittstelle

Je Partnersystem sollte ein separater API Benutzer erstellt werden, damit im ERP selber konfiguriert werden kann, welches Partnersystem welche Daten erhalten soll.

Mehr Details finden Sie im UTS KARTHAGO Handbuch.

## API Zugänge

In dem **API Zugänge** Modul werden die Zugangsdaten für die Anbindung an Aareon Connect hinterlegt. Im oberen Teil des Moduls ist zunächst die gewünschte Token-Nummer einzutragen. Danach teilt sich die Maske in die Bereiche Token und Objekt-Rechte auf. Als Erstes ist auf dem Reiter Token die Bezeichnung und der Gültigkeitszeitraum des Tokens zu erfassen, wobei das Enddatum leer gelassen werden kann. Das Aktiv-Kennzeichen ist nur bei Token zu entfernen, die nicht mehr verwendet werden sollen. Bei der Art des Tokens müssen Sie **REST** auswählen:

Diese Art wird für die Anbindung an Aareon Connect verwendet. Bei dieser Art stellt sich der untere Teil der Maske wie folgt dar, wo dann die weiteren erforderlichen Angaben zu erfassen sind:

<figure><img src="../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

Bevor nun als Zweites die Objektzuordnung vorgenommen werden kann, ist der Datensatz zu speichern. Anschließend ist wieder in den Änderungsmodus und auf den Reiter Objekt-Rechte zu wechseln. Auf dem Reiter werden die Objekte festgelegt, für die der jeweilige Token gelten soll. Mittels des Buttons **Objekt(e) hinzufügen** werden die Objekte dem Token hinzugefügt. Je nach Art des Tokens können in der Objektauswahl unterschiedliche Festlegungen getroffen werden.

Bei **REST** stellt sich die Objektauswahl wie folgt dar:

<figure><img src="../.gitbook/assets/image (61).png" alt="" width="563"><figcaption></figcaption></figure>

Es kann festgelegt werden, welche Rechte (Lesen/Schreiben/Löschen) bei den einzelnen Objekten für verschiedene Bereiche eingetragen werden sollen. Sollen sämtliche Rechte eingetragen werden, kann auch der Button **Alles auswählen** verwendet werden. Die hinzugefügten Objekte werden dann auf der Hauptmaske dargestellt:

<figure><img src="../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

Wenn neue Objekte angelegt werden, die ebenfalls übertragen werden sollen, sind diese manuell hinzuzufügen bzw. Objekte, die nicht mehr übertragen werden sollen, manuell zu entfernen.

{% hint style="info" %}
Werden bei einem API Zugang für Aareon Connect neue Objekte hinzugefügt, Änderungen an bestehenden Objekteinträgen oder Objekte entfernt, wird bei den Objekten das Änderungsdatum angepasst, so dass bei der nächsten Übertragung nach Aareon Connect die geänderten Objekte beachtet werden.
{% endhint %}

## Use Cases

### Allgemein

* Bei allen Use Cases werden die Mandanten direkt im ERP System für die Schnittstelle freigegeben.\
  Deswegen, gibt es bei den UTS KARTHAGO Integrationen keine Mandanten Filterung bei der Aareon Connect Aktivierung selber.
* In UTS KARTHAGO gibt es keine Wirtschaftseinheiten, entsprechend sind alle Einstellungen dazu in allen Use Cases für UTS KARTHAGO irrelevant

### Stammdaten

#### Entitäten

| Aareon Connect Standard                                        | UTS KARTHAGO |
| -------------------------------------------------------------- | ------------ |
| [Wirtschaftseinheiten](../entitaeten/wirtschaftseinheiten.md)  | N/A          |
| [Gebäude](../entitaeten/gebaeude.md)                           | Objekte      |
| [Verwaltungseinheiten](../kategorien/eigentuemerverwaltung.md) | Einheiten    |
| [Mietverträge](../entitaeten/mietvertraege.md)                 | Verträge     |
| [Mieter](../entitaeten/mieter.md)                              | Mieter       |
| [Eigentümerverträge](../entitaeten/eigentuemervertraege.md)    | Verträge     |
| [Eigentümer](../entitaeten/eigentuemer.md)                     | Eigentümer   |

#### Besonderheiten

* Mietkosten werden bei UTS KARTHAGO nicht übertragen, entsprechend sind alle Einstellungen dazu für UTS KARTHAGO irrelevant

### Dokumente

#### Entitäten

| Aareon Connect Standard | UTS KARTHAGO |
| ----------------------- | ------------ |
| Archive                 | N/A          |
| Ordner                  | Ordner       |
| Dokumente               | Dokumente    |

#### Besonderheiten

* Nicht synchronisiert werden Dokumente, die
  * mit Adressen verknüpft sind
  * keine Ordnerzuordnung haben
  * größer als 50MB sind ([allgemeine Einschränkung des Dokumenten Use Cases](../use-cases/dokumente.md#einschraenkungen) für alle ERPs)
* Der Freigabestatus von Dokumenten wird aktuell nicht übermittelt, stattdessen werden alle synchronisierten Dokumente werden als "nicht freigegeben" behandelt

#### API Dokumentfreigaben

In der Dokumentenverwaltung können die Ordner definiert werden, aus denen die Dokumente nach Aareon Connect exportiert werden sollen. Die Definition wird mittels des im Ordnerbereich aufzurufenden Kontextmenüs vorgenommen. In diesem ist der Menüpunkt API Zugang Ordner freigeben zu selektieren:

<figure><img src="../.gitbook/assets/image (64).png" alt="" width="351"><figcaption></figcaption></figure>

Es öffnet sich dann eine neue Maske:

<figure><img src="../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

In dem Bereich API Zugang ist zunächst die API Einstellung mit der entsprechenden Bezeichnung auszuwählen und dann in den Änderungsmodus zu wechseln. Jetzt können die Ordner markiert werden, aus denen die Dokumente exportiert werden sollen. Die globalen Ordner, d. h. die die in allen Bereichen zur Verfügung stehen, sind mit folgendem Symbol gekennzeichnet: ![](<../.gitbook/assets/image (67).png>)

Nach Selektion der gewünschten Ordner, sind die Einstellungen zu speichern.

{% hint style="warning" %}
Werden nachträglich neue Ordner angelegt, ist bei diesen standardmäßig die Exportoption nicht gesetzt, d. h. diese muss gegebenenfalls direkt nach der Anlage des neuen Ordners gesetzt werden.
{% endhint %}
