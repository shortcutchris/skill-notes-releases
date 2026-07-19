# Skill Notes 0.7.0

Skill Notes can now keep your local-first vault up to date across Macs through
your private iCloud database.

Enable sync from the new iCloud Settings pane. Before anything is sent, Skill
Notes shows the number of local notes and attachments plus their aggregate
size. Notes remain ordinary Markdown and JSON files on every Mac and continue
working offline or after sync is disabled.

The All Notes window stays quiet while synchronization is healthy. A compact
status appears only while changes are moving or when an account or transfer
needs attention, and opens the relevant iCloud settings directly.

The synchronized vault includes notes, attachments, revision history,
workspaces, custom skills, favorite-skill presentation, portable preferences,
and stable local-model choices. Note content and file payloads use encrypted
CloudKit fields and assets. Every downloaded file is verified before it
replaces a local file. A note can arrive before a later attachment batch, but
an attachment appears in its metadata only when the verified payload is
installed atomically.

Conflict handling is intentionally conservative. Concurrent note bodies create
a clearly named conflict copy, and a later offline edit survives a remote
deletion as a conflict copy. Concurrent replacements of the same attachment
keep both verified files with a localized conflict name. Encrypted attachment
and revision identities are cross-checked against the independently verified
asset before local changes are applied. Account changes pause sync and preserve
local data until you explicitly adopt the current Apple Account.

Model binaries remain local to each Mac. The model ID and download/preload
policy can synchronize; missing GGUF and Whisper models are then offered in
Settings or downloaded automatically on an unmetered connection. Background
downloads retain progress across Settings reconstruction, check free space
before transfer, verify pinned GGUF files by SHA-256, reject corrupt partial
files, and never switch an unavailable local workflow to OpenAI.

Local deletion and iCloud deletion are separate confirmed actions. Deleting
local data first detaches sync and leaves the iCloud vault untouched; deleting
the synced iCloud vault keeps this Mac's local files.

The production path has been exercised end-to-end across two Macs, including
push delivery without a manual sync, a deliberately interrupted 16 MiB
attachment transfer with recovery, locked-screen state reopening, offline
edits, and concurrent conflict preservation.

Compatibility: macOS 14 or later.
