# Skill Notes 0.9.5

This update makes iPhone-to-Mac handoff both faster to understand and more
predictable.

## Highlights

- Favoriting a note on iPhone reveals it on the Mac and keeps it pinned above
  ordinary windows.
- **Show on Mac** also works for non-favorite notes and brings them forward
  once without silently favoriting them.
- Handoff is enabled by default on new Mac installations, while a deliberate
  per-Mac opt-out remains respected.
- Favorite and manual requests continue to use the immediate CloudKit and APNs
  fast path, retain offline retry, and add no timer or polling loop.
- Out-of-order delivery is safe: a favorite request waits until the pinned note
  revision is present before the window appears.

The matching iPhone behavior is delivered independently through TestFlight.

---

# Skill Notes 0.9.5

Dieses Update macht die Übergabe vom iPhone zum Mac verständlicher und
verlässlicher.

## Highlights

- Wird eine Notiz auf dem iPhone favorisiert, erscheint sie auf dem Mac und
  bleibt dort über normalen Fenstern angeheftet.
- **Auf dem Mac anzeigen** funktioniert auch für nicht favorisierte Notizen
  und holt sie einmalig nach vorn, ohne sie unbemerkt zu favorisieren.
- Die Übergabe ist auf neuen Mac-Installationen standardmäßig aktiv; eine
  bewusste Deaktivierung pro Mac bleibt erhalten.
- Favoriten- und manuelle Aufträge verwenden weiterhin den sofortigen
  CloudKit-/APNs-Schnellpfad, behalten die Offline-Wiederholung und benötigen
  weder Timer noch Abfrageschleifen.
- Auch eine abweichende Übertragungsreihenfolge ist sicher: Ein
  Favoritenauftrag wartet, bis die angeheftete Notizrevision vorhanden ist.

Das passende iPhone-Verhalten wird unabhängig über TestFlight ausgeliefert.
