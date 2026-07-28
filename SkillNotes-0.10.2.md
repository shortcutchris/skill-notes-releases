# Skill Notes 0.10.2

## English

### Instant iPhone handoff no longer waits for the main window

- Favorites and **Show on Mac** now load their exact encrypted CloudKit
  request and owning note as soon as the content-free relay signal arrives.
- The sticky note can appear while Skill Notes stays in the background; you
  no longer need to open All Notes or press **Sync Now** first.
- If CloudKit exposes the request just before the note, Skill Notes keeps the
  existing short, bounded retry active until the note is actually shown.
- The request ID and note relationship are verified before anything is
  applied through the existing conflict-safe synchronization path.

CloudKit remains the source of truth, and the relay still carries no note
identifier, title, body, tag, attachment, or other authored content.

---

# Skill Notes 0.10.2

## Deutsch

### Sofortige iPhone-Übergabe wartet nicht mehr auf das Hauptfenster

- Favoriten und **Auf dem Mac anzeigen** laden beim Eintreffen des
  inhaltsfreien Relay-Signals jetzt gezielt ihre verschlüsselte
  CloudKit-Anfrage und die zugehörige Notiz.
- Die Haftnotiz kann erscheinen, während Skill Notes im Hintergrund bleibt;
  vorheriges Öffnen von „Alle Notizen“ oder **Jetzt synchronisieren** ist
  nicht mehr erforderlich.
- Stellt CloudKit die Anfrage kurz vor der Notiz bereit, bleibt der bestehende
  kurze und begrenzte Wiederholungsablauf aktiv, bis die Notiz wirklich
  angezeigt wurde.
- Anfrage-ID und Notizbeziehung werden geprüft, bevor Daten über den
  bestehenden konfliktsicheren Synchronisierungsweg angewendet werden.

CloudKit bleibt die maßgebliche Datenquelle. Das Relay transportiert weiterhin
keine Notizkennung, Titel, Inhalte, Schlagwörter, Anhänge oder andere verfasste
Daten.
