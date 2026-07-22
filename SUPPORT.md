# Skill Notes Support

Skill Notes Mobile is an offline-first notes and tasks app for iPhone and iPad. It does not require a Skill Notes account.

## Before requesting support

1. Confirm that iOS or iPadOS is up to date.
2. In Skill Notes, check the sync status before changing iCloud settings.
3. For dictation, enable both **Microphone** and **Speech Recognition** for Skill Notes in system Settings.
4. If on-device speech recognition is unavailable for the selected language, type the note or task instead; Skill Notes does not silently fall back to cloud transcription.
5. Keep a copy of important exported Markdown or shared files before destructive troubleshooting.

## iCloud synchronization

iCloud synchronization is optional and uses the user's private CloudKit database. Confirm that the device is signed in to the intended Apple Account and that iCloud Drive is available. Disabling sync does not automatically delete local or cloud data.

## Dictation behavior

- **Note Dictation** inserts the raw transcript at the current insertion point and never creates tasks automatically.
- **Task Dictation** always opens an editable preview before creating tasks.
- Without a configured structuring model, the complete transcript remains exactly one editable task.

## Request support

Use the public [Skill Notes issue tracker](https://github.com/shortcutchris/skill-notes-releases/issues/new) and include:

- Skill Notes version and build number;
- iPhone or iPad model;
- iOS or iPadOS version;
- the exact steps that reproduce the problem; and
- what happened versus what you expected.

Do not post note contents, attachments, credentials, Apple Account details, diagnostic secrets, or other sensitive information in a public issue.

For privacy details, see the [Skill Notes Mobile Privacy Policy](PRIVACY.md).
