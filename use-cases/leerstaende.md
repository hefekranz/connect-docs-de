---
description: Synchronisierung von leerstehenden Einheiten aus dem ERP in das Partnersystem
---

# Leerstände

## Übersicht

* **Interval**: Maximal Stündlich
* **Richtung**: ERP -> Partnersystem
* **Entitäten**:
  * [Leerstände](../entitaeten/leerstaende.md)
* **Partner**:
  * [Immomio](../partner-and-apps/immomio.md)
  * [Wohnungshelden](../partner-and-apps/immomio.md)
  * [EverReal](../partner-and-apps/everreal.md)

## Wie aktiviere ich die Übertragung von Leerständen an meine Partnerlösung?

### Yuneo & Sigma

Damit die Leerstände aus dem ERP an Ihre Partnerlösung gesendet werden muss ein Job im ERP eingerichtet werden. Kontaktieren Sie hierzu bitte Ihren ERP Berater, der Ihnen zeigen kann wie die Einrichtung erfolgt.

### GAP, UTS KARTHAGO & RELion

Leerstände müssen im ERP freigegeben werden, damit Aareon Connect diese abrufen kann. Ihr ERP Berater zeigt Ihnen wie es funktioniert.

## Beschreibung

Die Synchronisation von Leerständen ermöglicht es Ihnen, **Daten über freie Verwaltungseinheiten zu übertragen**, die z.B. in einem System zur Verwaltung von Leerständen und Interessenten ausgeschrieben werden können.

Die Übertragung der Leerstände basiert bei allen ERPs und Partner Lösungen auf dem [OpenImmo 1.2.7b Format](http://www.openimmo.de/go.php/p/24/download.htm).

{% hint style="info" %}
Bei den Wodis ERPs wird der Interval über das ERP gesteuert ([mehr Details](../erps/wodis-yuneo.md#leerstande-und-interessenten)).
{% endhint %}
