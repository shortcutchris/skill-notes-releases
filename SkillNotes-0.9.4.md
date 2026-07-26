# Skill Notes 0.9.4

This update makes iPhone handoff faster and prevents false conflict notes.

## Highlights

- A fresh favorite or **Show on Mac** request is delivered through an explicit
  CloudKit push path instead of waiting for the normal background schedule.
- The Mac fetches the request immediately while remaining fully event-driven
  and idle when nothing changes.
- Sync now follows complete revision ancestry across several autosaves, so an
  older version cannot become a false conflict merely because it is more than
  one revision behind.
- Obsolete conflict copies that are proven ancestors move to Trash
  automatically. Real parallel edits remain safely preserved.

The matching iPhone improvement is delivered independently as TestFlight
Build 30.

---

# Skill Notes 0.9.4

Dieses Update beschleunigt die Übergabe vom iPhone und verhindert falsche
Konfliktnotizen.

## Highlights

- Ein neuer Favorit oder **Auf Mac anzeigen** wird über einen expliziten
  CloudKit-Push-Pfad übertragen, statt auf den normalen Hintergrundzeitplan zu
  warten.
- Der Mac lädt die Anfrage sofort und bleibt trotzdem vollständig
  ereignisgesteuert, solange sich nichts ändert.
- Die Synchronisierung verfolgt jetzt die vollständige Revisionskette über
  mehrere automatische Speicherungen. Eine ältere Version wird dadurch nicht
  fälschlich zum Konflikt, nur weil sie mehr als eine Revision zurückliegt.
- Veraltete Konfliktkopien, die nachweislich nur Vorfahren sind, wandern
  automatisch in den Papierkorb. Echte parallele Bearbeitungen bleiben sicher
  erhalten.

Die passende iPhone-Verbesserung wird unabhängig als TestFlight Build 30
bereitgestellt.
