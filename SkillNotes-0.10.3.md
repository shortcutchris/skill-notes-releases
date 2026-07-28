# Skill Notes 0.10.3

## English

### Sticky notes return to the right place

- General Settings can now remember every sticky note's position, size, and
  physical display independently on each Mac.
- Home restores those placements without overriding an active named
  workspace.
- If a saved display is temporarily unavailable, the complete note is mapped
  proportionally onto the main display instead of appearing off-screen.
- Disabling the setting pauses restoration and new position updates without
  deleting the positions already saved on that Mac.

### Agents can create visually formatted notes

- The local CLI and MCP server now accept the same canonical Markdown subset
  as the visual editor: headings 1–3, bold and italic emphasis, hyphen and
  numbered lists, checklists, and inline links.
- Input is canonicalized through one shared policy before the app writes it.
  Unsupported syntax, incomplete markers, and ambiguous delimiter
  combinations are rejected with a precise line and column instead of being
  stored in a damaged form.
- Existing typed task, attachment, workspace, permission, and stale-reference
  behavior remains unchanged.

Physical monitor positions remain local to each Mac and are never synchronized
to iPhone or iCloud. Agent access remains local, permission-controlled, and
routed through the running Skill Notes app as the only writer.

---

# Skill Notes 0.10.3

## Deutsch

### Haftnotizen kehren an die richtige Stelle zurück

- In den allgemeinen Einstellungen kann Skill Notes nun Position, Größe und
  physischen Monitor jeder Haftnotiz separat auf jedem Mac speichern.
- „Start“ stellt diese Positionen wieder her, ohne eine aktive benannte
  Arbeitsfläche zu überschreiben.
- Ist ein gespeicherter Monitor vorübergehend nicht verfügbar, wird die
  vollständige Notiz proportional auf den Hauptmonitor übertragen, statt
  außerhalb des sichtbaren Bereichs zu erscheinen.
- Wird die Einstellung deaktiviert, pausieren Wiederherstellung und neue
  Positionsspeicherungen, ohne bereits gespeicherte Positionen dieses Macs zu
  löschen.

### Agents können visuell formatierte Notizen erstellen

- Die lokale CLI und der MCP-Server akzeptieren jetzt denselben kanonischen
  Markdown-Umfang wie der visuelle Editor: Überschriften der Ebenen 1–3,
  Fett- und Kursivschrift, Aufzählungen und nummerierte Listen, Checklisten
  sowie Inline-Links.
- Eingaben werden vor dem Schreiben durch die App über eine gemeinsame Policy
  kanonisiert. Nicht unterstützte Syntax, unvollständige Marker und
  mehrdeutige Delimiter-Kombinationen werden mit genauer Zeile und Spalte
  abgewiesen, statt beschädigt gespeichert zu werden.
- Bestehende typisierte Aufgaben-, Anhang-, Arbeitsflächen-, Berechtigungs-
  und Veraltetheitsprüfungen bleiben unverändert.

Physische Monitorpositionen bleiben lokal auf dem jeweiligen Mac und werden
weder zum iPhone noch über iCloud synchronisiert. Der Agentenzugriff bleibt
lokal, berechtigungsgesteuert und verwendet die laufende Skill-Notes-App als
einzige Schreibinstanz.
