# Skill Notes 0.8.13

This reliability update fixes two background synchronization loops.

The local MCP connection used by Claude Code and other agents now refreshes
its tools only when the Skill Notes bridge itself changes. Routine status
checks no longer rewrite the activity history, while real note and task
operations remain visible there.

iCloud now resolves a record that already exists on the server through the
normal inbound merge before deciding whether another upload is needed.
Changes from another device therefore converge instead of remaining at 0 of N.
Data that genuinely requires repair pauses safely and remains stored locally
until an explicit retry.

## Deutsch

Dieses Zuverlässigkeitsupdate behebt zwei Synchronisationsschleifen im
Hintergrund.

Die lokale MCP-Verbindung für Claude Code und andere Agenten aktualisiert ihre
Werkzeuge nur noch, wenn sich die Skill-Notes-Verbindung selbst ändert.
Gewöhnliche Statusprüfungen schreiben nicht mehr in den Aktivitätsverlauf;
echte Notiz- und Aufgabenaktionen bleiben dort weiterhin sichtbar.

iCloud verarbeitet einen bereits auf dem Server vorhandenen Datensatz zuerst
über den normalen eingehenden Abgleich und entscheidet erst danach über einen
weiteren Upload. Änderungen von einem anderen Gerät laufen dadurch zusammen,
statt bei 0 von N stehen zu bleiben. Daten mit echtem Reparaturbedarf pausieren
sicher und bleiben bis zu einem ausdrücklichen neuen Versuch lokal erhalten.
