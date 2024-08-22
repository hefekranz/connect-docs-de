# GAP immotion

## Use Cases

### Stammdaten

Aus GAP immotion können Stammdaten in Partneranwendungen übertragen werden.

Die Adress- und Kommunikationsdaten wie Telefon, E-Mail-Adresse werden bidirektional ausgetauscht, dass heißt Änderungen in diesen Feldern in der Partneranwendung werden nach GAP immotion zurück übertragen.

Alle anderen Änderungen der Kontaktdaten wie z.B. Namensänderung, Änderung der Bankverbindung werden über den Use Case Tickets vorgenommen. An ein Ticket können auch Anhänge mit übergeben werden, z.B. bei Namensänderung könnte die Bescheinigung vom Einwohnermeldeamt mit gesendet werden.

### Tickets

In GAP immotion ist es möglich Tickets in einer sogenannten Vorgangsbearbeitung zu verwalten. Über die API können Tickets aus immotion an die Partnersysteme übertragen werden und es ist auch möglich aus einem Partnersystem Tickets nach immotion zu übertragen. Dabei können auch Anhänge an das Ticket angefügt werden.

In immotion werden Vorgangstypen z.B.: Mangel/ Reparatur definiert. Den Vorgangstypen können Adresstypen zugeordnet werden.

<figure><img src="../.gitbook/assets/Ticket-Adresstyp Zuordnung.png" alt=""><figcaption></figcaption></figure>

Bei Erstellung eines Ticket wird der sogenannte Aufgabenträger (Zuständigkeit zur Abarbeitung des Tickets) automatisch ermittelt.

<figure><img src="../.gitbook/assets/Ticket-Zuordnung Aufgabenträger.png" alt=""><figcaption></figcaption></figure>
