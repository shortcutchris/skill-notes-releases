# Skill Notes 0.11.0

## English

### More choice for cloud transcription

- OpenAI cloud dictation now offers the recommended `gpt-live-transcribe`
  model while keeping `gpt-realtime-whisper` selectable for established
  workflows.
- Supported audio and video attachments can be transcribed into a new,
  editable Meeting Note after explicit confirmation.
- File transcription supports `gpt-transcribe`,
  `gpt-4o-transcribe-diarize`, `gpt-4o-transcribe`,
  `gpt-4o-mini-transcribe`, and `whisper-1`. Speaker labels are retained when
  the selected model provides them.
- The exact model is fixed when a dictation or file transcription begins, so
  changing Settings cannot alter an active request. Portable model choices
  synchronize without credentials or recording contents.

### Empty tasks delete cleanly

- Pressing Backspace immediately after an empty checkbox now removes its
  complete task marker as one undoable action.
- Partial Markdown such as `• [ ]` is no longer exposed, and an already
  malformed empty marker is repaired by the same interaction.

Cloud transcription still runs only after an explicit user action. Note text,
recordings, and attachments are never sent to OpenAI merely because a model is
selected in Settings.

---

# Skill Notes 0.11.0

## Deutsch

### Mehr Auswahl bei Cloud-Transkriptionen

- Für OpenAI-Cloud-Diktate steht jetzt das empfohlene Modell
  `gpt-live-transcribe` zur Wahl; `gpt-realtime-whisper` bleibt für bestehende
  Abläufe auswählbar.
- Unterstützte Audio- und Videoanhänge lassen sich nach ausdrücklicher
  Bestätigung in eine neue, bearbeitbare Meeting-Notiz transkribieren.
- Für Dateitranskriptionen stehen `gpt-transcribe`,
  `gpt-4o-transcribe-diarize`, `gpt-4o-transcribe`,
  `gpt-4o-mini-transcribe` und `whisper-1` zur Verfügung. Sprecherangaben
  bleiben erhalten, wenn das gewählte Modell sie liefert.
- Das genaue Modell wird beim Start eines Diktats oder einer
  Dateitranskription festgehalten. Eine Änderung in den Einstellungen kann
  einen laufenden Auftrag daher nicht umstellen. Portable Modellauswahlen
  werden ohne Zugangsdaten oder Aufnahmeinhalte synchronisiert.

### Leere Aufgaben lassen sich sauber löschen

- Die Rücktaste direkt hinter einer leeren Checkbox entfernt jetzt den
  vollständigen Aufgabenmarker als eine rückgängig machbare Aktion.
- Markdown-Reste wie `• [ ]` werden nicht mehr sichtbar; auch ein bereits
  fehlerhafter leerer Marker wird mit derselben Bedienung bereinigt.

Cloud-Transkriptionen starten weiterhin nur nach einer ausdrücklichen Aktion.
Allein die Modellauswahl in den Einstellungen sendet weder Notiztext noch
Aufnahmen oder Anhänge an OpenAI.
