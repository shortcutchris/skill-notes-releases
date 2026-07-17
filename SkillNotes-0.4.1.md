# Skill Notes 0.4.1

This maintenance release fixes a workspace edge case that could leave Skill Notes running without a visible window.

When every note saved in the active workspace is currently in the Trash or otherwise unavailable, Skill Notes now opens All Notes automatically. The same safe fallback applies at launch, when reopening the app from the Dock, when opening a workspace, and when restoring the previous arrangement.

Workspace memberships are not removed by this fallback. Restoring a trashed note can therefore return it to its original workspace and saved placement.

No note content is changed or deleted by this update.

Compatibility: macOS 14 or later.
