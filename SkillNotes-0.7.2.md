# Skill Notes 0.7.2

This reliability update completes the main-actor boundary for synchronized
iCloud preferences.

Foundation and CloudKit may deliver preference notifications from a background
queue. Skill Notes now routes AI and dictation readiness, local-model runtime
stores, and AppKit localization observers through the same explicit main-actor
notification bridge before they inspect or update UI-owned state.

The regression path is covered with a background
`UserDefaults.didChangeNotification` delivered to a main-actor owner. The
complete observer audit removes equivalent actor-isolated Combine notification
sinks from app-owned main-actor classes.

No note, attachment, workspace, skill, preference, or iCloud data is removed
by this update.

Compatibility: macOS 14 or later.
