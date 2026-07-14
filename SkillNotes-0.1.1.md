# Skill Notes 0.1.1

This update makes note-scoped dictation easier to understand and much calmer inside a sticky note.

The Voice Pill now uses a compact, inset dark surface with white high-contrast typography instead of inheriting translucent colors from the note underneath. Its transcription badge clearly distinguishes local Apple Speech or Whisper from OpenAI cloud transcription, attached pills omit the redundant note title, and the panel adapts to narrow sticky-note windows.

After a raw transcript is inserted in Ask mode, the cleanup choices now say where processing happens: on this Mac or with OpenAI. Clicking either provider is the explicit invocation and begins the bounded cleanup immediately, without a second request-confirmation sheet. The completed result still appears in the normal review and cannot replace the transcript until Apply passes the existing exact-range and stale-result checks.

Cleanup providers preselected in Settings retain the full request review. Local cleanup never leaves the Mac; OpenAI cleanup contains only the inserted transcript range with zero surrounding characters, title, tags, or attachments.

Compatibility: macOS 14 or later.
