# Skill Notes 0.9.2

This maintenance update makes sequential visual formatting safe and
predictable in the macOS note editor.

## Highlights

- Bold → List → Bold off now produces a plain list item instead of exposing
  Markdown markers.
- The fix covers bulleted lists, numbered lists, and checklists while
  preserving the exact visible selection.
- Deleting at emphasis and link boundaries keeps the hidden canonical
  delimiters balanced and remains reversible in one Undo step.

Notes continue to use portable UTF-8 Markdown as their only stored body. This
update repairs selection translation between visible text and canonical source;
it does not change the storage or CloudKit schema.

---

# Skill Notes 0.9.2

Dieses Wartungsupdate macht aufeinanderfolgende visuelle Formatierungen im
macOS-Notizeditor sicher und vorhersehbar.

## Highlights

- „Fett → Liste → Fett aus“ erzeugt jetzt einen normalen Listeneintrag, statt
  Markdown-Zeichen sichtbar zu machen.
- Die Korrektur gilt für Aufzählungen, nummerierte Listen und Checklisten und
  bewahrt dabei exakt die sichtbare Textauswahl.
- Löschen an den Grenzen von Hervorhebungen und Links hält die unsichtbaren
  kanonischen Trennzeichen vollständig und bleibt mit einem Schritt
  rückgängig zu machen.

Notizen verwenden weiterhin portables UTF-8-Markdown als einzigen gespeicherten
Inhalt. Dieses Update repariert die Auswahlübersetzung zwischen sichtbarem Text
und kanonischer Quelle; Speicher- und CloudKit-Schema bleiben unverändert.
