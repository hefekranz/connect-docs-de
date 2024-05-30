# Umstellung DocuSign Integration

## Aktivierung in Aareon Connect

Mit der Migration von der Digitalen Unterschrift zu Aareon Connect, wird die Verbindung zwischen WODIS Sigma/SAP Blue Eagle und DocuSign über Locoia hergestellt, statt wie bisher über einen API Service von Aareon selber.

Dies ermöglicht die Migration zu [scrive-technologie-partner.md](scrive-technologie-partner.md "mention"), wodurch wir Ihnen neue Funktionen anbieten können ([#vorteile-scrive](scrive-technologie-partner.md#vorteile-scrive "mention")).

Als **DocuSign Bestandskunde** können Sie bis auf weiteres weiterhin DocuSign für die Digitale Unterschrift nutzen und müssen einmalig folgende Schritte für die Migration durchführen:

1. Öffnen Sie Aareon Connect in Ihrem ERP System ([mehr Details](../../#aareon-connect-per-video-verstehen))
2. Gehen Sie auf **DocuSign**
3. Geben Sie bei der Integration **Digitale Unterschrift mit DocuSign** die Zugangsdaten für den DocuSign Nutzter ein (muss ein Admin Nutzer sein), den Sie für die Integration verwenden möchten
   1.  Wir empfehlen, dass Sie einen Admin Nutzer speziell für die Integration nutzen um Probleme bei z.B. Passwort Änderung eines regulären Nutzers zu vermeiden

       <figure><img src="../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
4. Klicken Sie auf **Autorisieren**
   1. Die Nutzerdaten werden direkt überprüft und bei falschen Informationen erhalten Sie eine Meldung mit weiteren Informationen
5.  Suchen Sie nach dem DocuSign Account Namen den Sie verwenden wollen und suchen Sie den passenden Namen aus der Liste aus.\
    Wenn der Account Name nicht auftaucht, überprüfen Sie, dass Sie den Namen richtig eingegeben haben und das Sie sich in Schritt 4. erfolgreich autorisiert haben.

    <figure><img src="../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
6. Optional: Geben Sie die Bezeichnung der von Ihnen genutzten QES Identitätsüberprüfung an, mehr Details in [#nutzung-von-qes](umstellung-docusign-integration.md#nutzung-von-qes "mention")
7. Die Integration ist nun aktiviert
8. Sie erhalten somit in den kommenden Stunden via E-Mail die nötigen Informationen um die Integration im ERP System fertig einzurichten
9. Folgen Sie den Anleitungen der jeweiligen ERPs für die weiteren Einrichtungsschritte (Scrive kann dabei mit DocuSign ersetzt werden)

### Nutzung von QES

Mehr Details zu [#qualifizierte-elektronische-unterschrift](./#qualifizierte-elektronische-unterschrift "mention") finden Sie im verlinkten Artikel.

Um QES mit DocuSign nutzen zu können müssen Sie eine entsprechende "Identitätsüberprüfung" in Ihrem DocuSign Account haben.\
[Mehr Details dazu finden Sie hier bei DocuSign direkt](https://support.docusign.com/s/document-item?language=de\&rsc\_301=\&bundleId=pik1583277475390\&topicId=eya1583277454804.html&\_LANG=dede).

Um diese integriert Nutzen zu können müssen Sie den genauen Namen im 6. Schritt (Anleitung oben) eingeben.\
Den genauen Namen können Sie bei DocuSign unter **Einstellungen** > **Identitätsüberprüfung** sehen, wo sie die passende Identitätsüberprüfung aus der Liste auswählen können und diese dann so markieren und kopieren können:

<figure><img src="../../.gitbook/assets/Screenshot 2024-05-15 at 17.14.58.png" alt=""><figcaption></figcaption></figure>
