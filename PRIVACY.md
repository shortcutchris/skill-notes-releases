# Skill Notes Mobile Privacy Policy

Effective date: July 22, 2026

Skill Notes Mobile is designed to work without an account and to keep user-authored content under the user's control.

## Data the app handles

Notes, tasks, tags, workspaces, attachments, settings, and dictation transcripts are created for app functionality. By default, this content is stored locally in the app's container on the user's device.

Skill Notes does not use this content for advertising, analytics, profiling, or tracking. The app contains no third-party advertising or analytics SDKs.

## Optional iCloud synchronization

If the user explicitly enables synchronization, Skill Notes stores supported app data in the user's private CloudKit database in the `iCloud.com.skillnotes.app` container. The app does not operate a separate synchronization server. Private CloudKit data is associated with the user's Apple Account and is handled by Apple under the user's iCloud terms and settings.

Disabling synchronization does not silently delete either the local vault or the private CloudKit copy. Destructive recovery and deletion actions remain separate and explicit.

## Dictation

Dictation starts only after the user selects **Note Dictation** or **Task Dictation**. The app requests microphone and Speech Recognition permission for this purpose. Skill Notes requires Apple's on-device speech recognition for mobile dictation. Temporary microphone audio is not retained by Skill Notes after transcription.

Normal note dictation inserts text only. It never creates tasks automatically. Task dictation always shows an editable preview before any task is created.

## Data collection and tracking

Skill Notes Mobile:

- does not track users;
- does not show advertising;
- does not collect analytics or crash-reporting data through a developer-operated service;
- does not sell user data;
- does not link user-authored content to an advertising or analytics profile; and
- does not require a Skill Notes account.

## Retention and deletion

Local content remains on the device until the user deletes it through the app, removes the app and its local data, or uses an applicable system action. Data synchronized through iCloud remains subject to the user's explicit in-app actions and Apple Account/iCloud controls.

## Security

Skill Notes uses Apple platform protections, the app sandbox, private CloudKit storage, encrypted CloudKit fields for authored and structured payloads, and integrity checks for synchronized assets. No method of storage is guaranteed to be completely secure, so users should also protect access to their devices and Apple Accounts.

## Children

Skill Notes is a general productivity application and is not directed specifically at children. The app does not knowingly collect personal information through a developer-operated service.

## Changes to this policy

Material changes to the app's data practices will be reflected in this policy and in the App Store privacy information. The effective date above will be updated when the policy changes.

## Privacy questions

Open a private-data-free support request in the public [Skill Notes issue tracker](https://github.com/shortcutchris/skill-notes-releases/issues). Do not include note contents, attachments, credentials, Apple Account details, or other sensitive information in a public issue.
