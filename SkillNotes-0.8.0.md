# Skill Notes 0.8.0

Tasks now have a calm home without leaving their notes. The new Task Center
collects every Markdown checkbox across active sticky notes, supports filters,
collapsible source-note groups, priorities, calendar-only due dates, and writes
completion back to the exact source line. If a moved or deleted checklist line
leaves date or priority details behind, the Task Center lets you deliberately
reassign or discard them instead of guessing.

Local Agent Access is explicit and off by default. Depending on the chosen
permission, the bundled CLI and MCP stdio server can read, create, or safely
edit notes and tasks through the running app. Skill Notes remains the only
vault writer; credentials, deletion, AI execution, and authored activity-log
content remain outside this interface. Settings can install the signed helpers
without an administrator password, copy CLI/MCP configuration, test the local
bridge, inspect metadata-only activity, and revoke access immediately.

Task references are opaque and revision-bound, so an agent cannot accidentally
update a moved or changed checklist line. MCP inputs use strict schemas, large
bridge messages and attachments are bounded, concurrent writes are serialized,
and every local mutation reports its current iCloud scheduling state. The
bundled helpers are refreshed on every build, use Apple's Hardened Runtime,
and update together with the app.
