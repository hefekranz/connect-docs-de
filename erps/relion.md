# RELion One

## Aareon Connect in RELion One aktivieren

### Azure-Portal

Verwenden Sie das Azure-Portal, um die Aareon Connect Anwendung für Business Central bzw. RELion auf Ihrem Microsoft Entra Mandanten zu registrieren. Im Rahmen der Registrierung gewähren Sie den entsprechenden Diensten auch Zugriff auf die Anwendung. Der Zweck der Registrierung besteht darin, sicherzustellen, dass Business Central lokal und die Dienste die **Microsoft Entra ID-Details** des jeweils anderen kennen.

In den folgenden Schritten wird beschrieben, wie Sie eine neue Anwendung registrieren. Wenn Sie jedoch die **Microsoft Entra Authentifizierung** verwenden, haben Sie bereits eine registrierte Anwendung für Business Central.

Folgende Schritte müssen ausgeführt werden:

1.  Melden Sie sich beim Azure-Portal an, und registrieren Sie eine Anwendung für Aareon

    Connect im Microsoft Entra Mandanten.

    1.  Befolgen Sie die allgemeinen Richtlinien unter [Registrieren Ihrer Anwendung bei Ihrem](https://learn.microsoft.com/en-us/azure/active-directory/active-directory-app-registration)

        [Microsoft Entra Mandanten](https://learn.microsoft.com/en-us/azure/active-directory/active-directory-app-registration). Wenn Sie einem Microsoft Entra Mandanten eine Anwendung

        hinzufügen, müssen Sie die folgenden Informationen angeben:

        1.  **Name**:

            Geben Sie einen Namen für Ihre lokale Business Central-Lösung an, z. B. Aareon Connect
        2.  **Unterstützte Kontotypen**:

            Wählen Sie nur Konten in diesem Organisationsverzeichnis aus
        3.  **Umleitungs-URI**:

            Legen Sie das erste Feld auf **Web** fest, um eine Webanwendung anzugeben. Geben Sie die URL für Ihren RELion/ Business Central-Browser-Client ein, gefolgt von `OAuthLanding.htm`, zum Beispiel: `https://MyServer/BC230/OAuthLanding.htm` oder

            `https://RELion.dynamicstocloud.com/BC230/OAuthLanding.htm`

            1. _Bitte Beachten_: Die URL muss mit der URL des Webclients übereinstimmen, wie sie in der Browseradresse des Computers angezeigt wird, an dem Sie arbeiten. Auch wenn die tatsächliche URL beispielsweise lauten könnte, entfernt der Browser normalerweise die Portnummer.
    2. Nach Abschluss des Vorgangs wird im Portal eine Übersicht für die neue Anwendung angezeigt.
    3.  Kopieren Sie die **Anwendungs-ID (Client-ID)**, der die Anwendung zugewiesen wurde,

        sowie die von Ihnen angegebene Umleitungs-URL. Sie werden diese Informationen später

        verwenden.
2.  Erstellen Sie einen geheimen Clientschlüssel für die registrierte **Aareon Connect**

    Anwendung.

    1.  Befolgen Sie die allgemeinen Richtlinien unter [Hinzufügen von Anmeldeinformationen zu Ihrer](https://learn.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app#add-a-client-secret)

        [Webanwendung](https://learn.microsoft.com/en-us/azure/active-directory/develop/quickstart-register-app#add-a-client-secret)
    2. Bevor Sie die Seite **Zertifikate und Geheimnisse** verlassen, kopieren Sie den Wert des Geheimnisses (**Secret ID**) an einen temporären Speicherort. Auf den Wert kann nicht zugegriffen werden, sobald Sie die Seite verlassen. Sie benötigen diesen Schlüssel, um es später an das Aareon Connect Team zu kommunizieren.
3.  Erteilen Sie der registrierten Anwendung delegierte Berechtigungen für den Zugriff auf die

    erforderlichen Dienst-APIs (z. B. API.ReadWrite.all und Automation.ReadWrite.All für

    Dynamics 365 Business Central und User.Read für Microsoft Graph).

    Wählen Sie auf der Übersichtsseite der registrierten Anwendung **API-**

    **Berechtigungen** > **Berechtigung hinzufügen** aus. Verwenden Sie dann den Bereich **API-**

    **Berechtigungen anfordern**, um die API zu suchen und Berechtigungen hinzuzufügen.

    1. Weitere Informationen finden Sie unter [Hinzufügen von Berechtigungen für den Zugriff auf Web-APIs](https://learn.microsoft.com/en-us/azure/active-directory/develop/quickstart-configure-app-access-web-apis#add-permissions-to-access-web-apis) in der Azure-Dokumentation.
4.  Konfigurieren Sie die Zustimmung für jede API-Berechtigung gemäß den Richtlinien Ihrer

    Organisation.

    1.  Die Zustimmung ist ein Prozess, bei dem Benutzer oder Administratoren einer Anwendung

        den Zugriff auf eine Ressource autorisieren, z. B. das Profil oder das Postfach eines

        Benutzers, je nach Dienst. Wenn ein Benutzer zum ersten Mal versucht, sich bei der

        registrierten App anzumelden, fordert die App die Berechtigung an, und der Benutzer muss

        zustimmen, um fortzufahren. Als Administrator können Sie im Namen aller Benutzer

        zustimmen, damit sie dies nicht tun müssen.
    2.  Weitere Informationen finden Sie unter [Weitere Informationen zu API-Berechtigungen und](https://learn.microsoft.com/en-us/azure/active-directory/develop/quickstart-configure-app-access-web-apis#more-on-api-permissions-and-admin-consent)

        [Administratoreinwilligung](https://learn.microsoft.com/en-us/azure/active-directory/develop/quickstart-configure-app-access-web-apis#more-on-api-permissions-and-admin-consent) und [Einführung in Berechtigungen und Einwilligung](https://learn.microsoft.com/en-us/azure/active-directory/develop/permissions-consent-overview).

### Einrichtung in RELion

1. Nachdem Sie die Anwendungsregistrierung erstellt haben, besteht die nächste Aufgabe darin, den Business Central-Mandanten für die Verwendung zu konfigurieren.
2. Sie benötigen die folgenden Informationen zur Anwendungsregistrierung:
   1. Umleitungs-URL
   2. Anwendungs-ID (Client-ID)
   3. geheimer Clientschlüssel.
3. Zudem benötigen Sie Informationen zur App RELion Aareon Connect.
   1. Dazu wählen Sie in Business Central die Suche (Lupe in der rechten oberen Ecke) aus und geben Sie Erweiterungsverwaltung ein.
   2. Aus der Liste Aareon Connect auswählen.
   3. Die Seite in die maximale Breite vergrößern, um Informationen komplett zu sehen.
   4. Notieren Sie sich die App-ID und den Name.
4. Danach die folgenden Schritte:
   1. Wählen Sie in der oberen rechten Ecke das 🔍 Symbol aus, geben Sie **Microsoft Entra Anwendungen** ein und wählen Sie dann den zugehörigen Link aus.
   2. Wählen Sie **Microsoft Entra Anwendungen** aus. Die Seite **Microsoft Entra Anwendungen** wird geöffnet.
   3. Wählen Sie den Menüpunkt **Neu** aus.
   4. Geben Sie im Feld **Client ID** die Anwendungs-ID (Client-ID) der **Aareon Connect**-Anwendung in Microsoft Entra-ID an, die Sie in der vorherigen Aufgabe kopiert haben.
   5. Geben Sie im Feld **Beschreibung** Aareon Connect ein.
   6. Geben Sie im Feld **App-ID** unter Extension, die ID des **Aareon Connect** ein und im Feld **App-Name**, der Name des **Aareon Connects**.
   7. _Bitte Beachten_: Unter **User Information** wird automatisch eine Benutzer ID und einen Benutzername definiert.
   8.  Im Inforegister **Benutzerberechtigungssätze** wählen Sie bitte folgende Berechtigungssätze

       aus:

       1. D365 AUTOMATION
       2. EXTEN. MGT. – ADMIN
       3. RELion Berechtigungssätze
   9. Die **Aareon Connect Anwendung** ist nun registriert und bereit, eine Verbindung mit dem Aareon Connect Partnersystem herzustellen.
   10. Bitte Ihren Ansprechpartner für die Integration informieren und über gesicherte Wege die Informationen (Client-Id, Client-Secret, Redirect URI usw.) zur Verfügung stellen um das Partnersystem via Aareon Connect mit RELion kommunizieren kann.
