# Skill Notes 0.7.1

This reliability update fixes a crash that could occur immediately after
enabling iCloud sync.

CloudKit can notify applications about changed preferences from a background
XPC queue. Skill Notes now moves that notification through an explicit
main-actor boundary before it updates the global Quick Note shortcut or other
AppKit state. The same path is covered by a regression test that posts the
notification from a background task.

Synchronized preference changes also no longer trigger repeated online
Whisper catalog requests. Background model policy checks inspect installed
assets only, coalesce bursts, preserve an evaluation already in progress, and
avoid rewriting unchanged local model paths. Opening the model library in
Settings continues to refresh the optional online catalog normally.

No note, attachment, workspace, skill, or iCloud data is removed by this
update.

Compatibility: macOS 14 or later.
