# Skill Notes 0.2.0

This release introduces named note workspaces: reusable spatial arrangements for the sticky notes that belong together.

A workspace remembers which sticky notes are visible, their positions and sizes on each display, front-to-back order, minimized state, and whether each note is pinned. Workspaces live in the secondary All Notes window and in a dedicated macOS app menu, with optional `⌥⌘1` through `⌥⌘9` shortcuts. The sticky-note toolbar remains calm and uncluttered.

Switching is reversible with one-step arrangement restore. If a saved display is unavailable, windows are proportionally placed and clamped onto an available screen. A note with active dictation or an open AI-result review is never hidden silently. Deleting a workspace removes only its spatial arrangement and never deletes notes, revisions, or attachments.

Workspace state is local spatial metadata only. It contains note identifiers and window geometry, never note text, and creating or switching a workspace does not contact an AI provider.

The All Notes workspace controls have compact native hit targets, clear Active and Modified states, complete English and German localization, and deterministic restoration after relaunch. Export and Delete All now include the versioned workspace document.

This update also removes recursive menu-localization work that could otherwise keep the main thread and WindowServer busy. With multiple open sticky notes, the verified idle app remains below one percent CPU. The Mac Studio release workflow now reports failed builds reliably and falls back to its verified Tailscale address if MagicDNS is temporarily unavailable.

Compatibility: macOS 14 or later.
