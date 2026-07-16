# Skill Notes 0.3.0

This release makes named workspaces much easier to understand and organize directly from the All Notes overview.

Notes can now be dragged onto a workspace in the sidebar. This always adds a membership rather than moving the note away from another workspace. Each note displays its saved workspace memberships, every workspace shows its note count, and the contextual Workspaces menu provides the same add/remove controls for keyboard and assistive-technology use. Each successful change has immediate feedback and one-step Undo.

Closed notes can be assigned without being opened first. Skill Notes restores their last saved sticky-window frame when possible and otherwise creates a safe cascaded position within the current display. When the target workspace is already open, only the affected note appears or hides; unrelated live window changes remain untouched.

Workspace controls now describe exactly what will happen. An inactive workspace offers Open Workspace, an active saved workspace shows Workspace Open, and a modified active workspace offers Save Changes or Restore Saved Layout. This prevents an inactive workspace from being overwritten accidentally.

Notes with active dictation or an open AI-result review remain protected. Removing one from the active workspace requires explicit confirmation before its saved membership changes while the active note stays visible.

Workspace data remains local spatial metadata only. Dragging or assigning a note never reads or transmits its content and does not invoke an AI provider.

Compatibility: macOS 14 or later.
