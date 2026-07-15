# Skill Notes 0.2.2

This follow-up patch release contains the same deterministic local-AI shutdown protection introduced in 0.2.1 and validates the complete Sparkle handoff from a running version that already includes that protection.

When Skill Notes quits for an update, active local model preparation, text generation, and Whisper transcription are cancelled and joined before llama.cpp and Core ML resources are released. AppKit completes termination only after that cleanup finishes.

There are no additional note, skill, dictation, privacy, or model-behavior changes from 0.2.1.

Compatibility: macOS 14 or later.
