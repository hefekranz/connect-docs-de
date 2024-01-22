# Umstellung DocuSign Integration

Mit der Migration von der Digitalen Unterschrift zu Aareon Connect, wird die Verbindung zwischen WODIS Sigma/SAP Blue Eagle und DocuSign über Locoia hergestellt, statt wie bisher über einen API Service von Aareon selber.

{% hint style="warning" %}
Für einen Unterbrechungsfreien Ablauf sollten die unteren Schritte bis zum **TBD** durchgeführt werden. Die Integration wird dann am **TBD** im Hintergrund für Sie zu Locoia umgestellt.
{% endhint %}

Dies ermöglicht die Migration zu [scrive-technologie-partner.md](scrive-technologie-partner.md "mention"), wodurch wir Ihnen neue Funktionen anbieten können ([#vorteile-scrive](scrive-technologie-partner.md#vorteile-scrive "mention")).

Als **DocuSign Bestandskunde** können Sie bis auf weiteres weiterhin DocuSign für die Digitale Unterschrift nutzen und müssen einmalig folgende Schritte für die Migration durchführen:

1. Öffnen Sie Aareon Connect in Ihrem ERP System ([mehr Details](../../#aareon-connect-per-video-verstehen))
2. Gehen Sie auf **DocuSign**
3. Geben Sie bei der Integration **Digitale Unterschrift mit DocuSign** die Zugangsdaten für den DocuSign Nutzter ein (muss ein Admin Nutzer sein), den Sie für die Integration verwenden möchten
   1.  Wir empfehlen, dass Sie einen Admin Nutzer speziell für die Integration nutzen um Probleme bei z.B. Passwort Änderung eines regulären Nutzers zu vermeiden\


       <figure><img src="../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
4. Klicken Sie auf **Autorisieren**
   1. Die Nutzerdaten werden direkt überprüft und bei falschen Informationen erhalten Sie eine Meldung mit weiteren Informationen
5. Die Integration ist nun aktiviert
6. Sie erhalten somit in den kommenden Stunden via E-Mail die nötigen Informationen um die Integration im ERP System fertig einzurichten
7. Folgen Sie den Anleitungen der jeweiligen ERPs für die weiteren Einrichtungsschritte (Scrive kann dabei mit DocuSign ersetzt werden)
