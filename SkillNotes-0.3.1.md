# Skill Notes 0.3.1

This release keeps the All Notes toolbar visually stable and finishes the German/English consistency pass across AI and dictation surfaces.

The search field now stays in one window-level toolbar position when the sidebar is shown or hidden. A dedicated localized sidebar button makes the layout transition predictable without moving or resizing search.

AI and dictation readiness now uses consistent wording in the sticky-note badge, readiness popover, AI Settings, provider previews, offline messaging, model loading states, failures, and the update channel. German mode no longer mixes English status terms such as “AI ready”, “Text skills”, or “Transcription” into those dynamic surfaces.

New regression coverage compares the English and German catalogs, flags unexpectedly untranslated German values, detects dynamic English literals that bypass localization, and verifies the affected toolbar and readiness interactions in the runnable app.

Compatibility: macOS 14 or later.
