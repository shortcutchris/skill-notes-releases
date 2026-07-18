# Skill Notes 0.6.1

Attachment dragging is now predictable, reversible, and calm in both sticky notes and All Notes.

The attachment control stays under the pointer when details open or close. Sticky-note details grow upward; library details grow downward. Press Escape after working in the file collection to close it again.

Drag behavior now has explicit source and destination semantics:

- dropping back onto the same note does nothing;
- dropping onto another note copies in Keep mode;
- dropping onto another note moves only after the target copy succeeds in Remove mode;
- dropping into Finder or another app exports the file, and removes the note-owned copy only when Remove mode is selected and the destination accepts it;
- cancelled, rejected, or partial drops never remove the source.

Successful Remove-mode operations show a confirmation with Undo. Undo restores an externally exported attachment, or restores the source and removes the just-imported target copy after a note-to-note move.

Attachment dragging no longer competes with workspace-row dragging or moves its sticky-note window.

CloudKit synchronization remains disabled in this release. Its opt-in migration is now an explicit deferred Phase 6 after the attachment and library experience is fully stabilized.

Compatibility: macOS 14 or later.
