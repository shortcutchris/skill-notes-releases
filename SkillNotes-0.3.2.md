# Skill Notes 0.3.2

This release cleans up two visual inconsistencies in the All Notes window.

The duplicate automatic sidebar toggle and its vertical separator have been removed from the middle of the toolbar. The dedicated Skill Notes sidebar control stays at the leading edge, while the search field remains anchored when the sidebar changes.

The compact New Workspace plus now sits directly beside the Workspaces heading instead of being pushed to the far edge of the sidebar.

UI regression coverage verifies the single-toggle hierarchy, stable search position, inline workspace action placement, and workspace creation entry point. The remote test workflow also strips copied provenance metadata before building so macOS does not interrupt XCTest with an unrelated Gatekeeper prompt.

Compatibility: macOS 14 or later.
