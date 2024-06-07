---
description: >-
  Synchronisierung von Archiven, Ordnern und Dokumenten aus dem ERP in das
  Partnersystem
---

# Dokumente

## Übersicht

* **Interval**: 3x pro Woche / Echtzeit
* **Richtung**: ERP -> Partnersystem
* **Entitäten**:
  * Archive
  * Ordner
  * Dokumente
* **Partner**:
  * [facilioo.md](../partner-and-apps/facilioo.md "mention")
  * [idwell.md](../partner-and-apps/idwell.md "mention")
  * [spiri.bo.md](../partner-and-apps/spiri.bo.md "mention")

## Beschreibung

Der Dokumente Use Case umfasst die Synchronisation von Archiven, Ordnern und Dokumenten in die jeweiligen Partnersysteme.

Dabei werden die Archiv und/oder Ordnerstrukturen aus dem ERP im Partnersystem gespiegelt (tägliche Aktualisierung).\
Die Dokumenten Speicherung funktioniert je nach Partnersystem unterschiedlich:

1. **Echtzeit-Abruf**: Im Partnersystem werden Datei-Metadaten (z.B. Titel, Erstellungsdatum) abgespeichert und beim Anklicken einer Datei in dem Partnersystem, wird das Dokumente vom jeweiligen ERP in Echtzeit abgerufen und im Partnersystem angezeigt
2. **Speicherung im Partnersystem**: Die Dateien werden im Partnersystem selber gespeichert und bei der täglichen Aktualisierung bei Änderungen entsprechend aktualisiert

## Einschränkungen

Dokumente die größer als 50MB sind, werden nicht synchronisiert.
