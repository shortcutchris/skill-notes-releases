# Skill Notes 0.9.6

This update makes Workspaces reversible and iPhone-to-Mac favorites independent
of the overview window.

## Highlights

- **Home** is a permanent system destination that returns to the standard
  all-notes mode. It cannot be renamed or deleted.
- Global favorites remain visible, unminimized, and above ordinary windows
  even while a named workspace is active.
- CloudKit push events now finish their immediate fetch before applying
  inbound changes, including pushes received while the sync engine is still
  starting or already fetching.
- Favoriting on iPhone can reveal the synchronized note without first opening
  or focusing the All Notes window.
- Launch restores every favorite, including favorites outside the last active
  named workspace.

The matching iPhone behavior remains independently delivered through
TestFlight.

---

# Skill Notes 0.9.6

Dieses Update macht Arbeitsflächen umkehrbar und Favoriten vom iPhone
unabhängig von der Notizübersicht.

## Highlights

- **Start** ist ein dauerhaftes Systemziel und kehrt zum normalen Modus mit
  allen Notizen zurück. Es kann weder umbenannt noch gelöscht werden.
- Globale Favoriten bleiben auch bei einer aktiven benannten Arbeitsfläche
  sichtbar, nicht minimiert und über normalen Fenstern.
- CloudKit-Pushs schließen nun ihren sofortigen Abruf ab, bevor eingegangene
  Änderungen übernommen werden – auch während die Sync-Engine startet oder
  bereits Daten lädt.
- Ein auf dem iPhone gesetzter Favorit kann die synchronisierte Notiz anzeigen,
  ohne dass zuerst die Übersicht „Alle Notizen“ geöffnet oder fokussiert wird.
- Beim Start werden alle Favoriten wiederhergestellt, auch außerhalb der
  zuletzt aktiven benannten Arbeitsfläche.

Das passende iPhone-Verhalten wird weiterhin unabhängig über TestFlight
ausgeliefert.
