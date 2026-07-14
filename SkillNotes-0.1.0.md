# Skill Notes 0.1.0

This is the first signed public Skill Notes release (build 8). Future updates are delivered through the public `shortcutchris/skill-notes-releases` Sparkle feed while the application source remains private.

This unreleased preview establishes the complete local-first product foundation: independent floating sticky notes, ten contrast-safe color pairs, Markdown storage, search and organization, revisions, attachments, declarative skills, exact selection replacement, safe previews, onboarding, preferences, transparent export/delete, the final 3D app icon, and optional OpenAI Responses API transformations.

It also introduces note-scoped voice dictation: on-device by default, optionally powered by OpenAI Realtime, with a persistent floating Voice Pill, exact cursor/selection insertion, one-step undo, explicit cleanup, and safe lifecycle handling when the note loses focus, minimizes, closes, or becomes stale.

OpenAI dictation now opens the correct Realtime transcription-intent WebSocket and configures `gpt-realtime-whisper` as the input transcription model, fixing sessions that previously ended without text. The captured insertion caret is also slimmer, shorter, and vertically centered against the active text line.

The Voice Pill now docks to the visible target note as a native child window, so it follows every note drag and resize synchronously. It detaches only when the note is minimized or unavailable, keeping recording controls reachable without losing the captured insertion target.

Editor preferences now include five curated native font families with multiple serif options and a live preview. Sticky-note color menus display the real background/typography pair, and up to two skills can be pinned directly in every note toolbar. Pinning a third skill promotes it immediately and replaces the least recent toolbar favorite.

Pinned skills are now true quick actions: one click sends the captured Selection or Whole Note target immediately. The returned text still appears in the normal result preview and cannot change the note until Apply passes the exact stale-result and range checks.

The app bundle embeds the custom 3D icon through the modern asset catalog as its single source of truth, so Dock, Finder, Launchpad, About, and LaunchServices resolve the same artwork without a conflicting legacy resource.

The entire app-owned interface now ships in English and German. General Settings switches language immediately across already open sticky notes, All Notes, Settings, onboarding, skill and dictation workflows, dialogs, window titles, and menu commands without a relaunch. Open editor/workflow state is preserved, and note text, titles, tags, custom skills, and provider output are never translated automatically. A central language registry and key-parity tests keep future language additions additive.

Settings now includes a dedicated Changelog pane. It identifies the running version and build, renders the complete bundled Markdown release history offline, switches immediately between the English and German documents, and safely falls back to English when a future language does not yet have a translated changelog.

AI can now be completely local. AI Settings switches text skills live between OpenAI and embedded llama.cpp, with curated Qwen and Gemma GGUF downloads, explicit selection, progress, cancellation, and deletion. Dictation adds downloadable WhisperKit alongside Apple Speech and OpenAI Realtime. Local generation and transcription require no account, background server, or note-content transmission; provider snapshots prevent an already reviewed request from being rerouted after a Settings change.

The embedded llama.cpp package is pinned to a reviewed compatibility commit that exports its image-decoding C shims with the correct ABI. This keeps the universal Developer ID archive reproducible for both Apple silicon and Intel Macs without changing the local text-model behavior.

All microphone providers now cross the AVAudioEngine realtime boundary through explicit nonisolated, sendable bridges. This prevents Swift actor-isolation assertions from terminating the app when recording starts, including the previously reproducible WhisperKit crash.

Local prompts are tailored for compact instruction models and streamed output removes internal reasoning and request-boundary markers even when a tag is split across tokens. Live integration coverage requires the model to perform an actual grammar correction, not merely return non-empty output.

Compatibility: macOS 14 or later.

Privacy: ordinary note work stays local. Local text and Whisper providers keep prompts and audio on the Mac. Palette requests show the exact payload before approval; toolbar favorites send the same bounded payload after their explicit click. OpenAI response storage is disabled, partial output cannot be applied, and signed builds keep the user-owned key in macOS Keychain.

Skill schema: version 1 is declarative JSON only. Imports are validated and never overwrite an existing skill silently.
