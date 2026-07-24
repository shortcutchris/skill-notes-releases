# Skill Notes 0.8.11

This release keeps sequentially created checklist items distinct in the Task
Center.

Every new task now receives an identity that remains unique even though a
continued checklist line starts out empty. Existing notes that contain legacy
identity collisions repair themselves deterministically when loaded. The
repair changes no Markdown text, completion state, due date, or priority.

iCloud metadata merging applies the same normalization before combining task
details, so older synchronized notes remain safe and display each task with
its own title.

The local agent bridge is also ready before asynchronous window restoration
finishes, so enabling and testing agent access immediately after launch no
longer leaves Settings at Unavailable.

## Deutsch

Dieses Release stellt nacheinander angelegte Checklistenpunkte in der
Aufgabenansicht wieder eindeutig dar.

Jede neue Aufgabe erhält jetzt eine eigene Identität, auch wenn eine
fortgesetzte Checklistenzeile zunächst leer entsteht. Bereits vorhandene
Notizen mit alten ID-Kollisionen reparieren sich beim Laden deterministisch.
Markdown-Text, Erledigt-Status, Fälligkeit und Priorität bleiben unverändert.

Auch der iCloud-Metadatenabgleich normalisiert solche alten Kollisionen vor dem
Zusammenführen, damit jede synchronisierte Aufgabe ihren eigenen Titel behält.

Die lokale Agentenverbindung ist außerdem bereits vor dem Abschluss der
asynchronen Fensterwiederherstellung bereit. Wird der Agentenzugriff direkt
nach dem Start aktiviert und getestet, bleibt der Status nicht mehr bei
„Nicht verfügbar“ stehen.
