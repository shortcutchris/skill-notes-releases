# Skill Notes 0.2.1

This patch release fixes a crash that could be reported after Sparkle installed an automatic update while a local AI model had been loaded.

Skill Notes now keeps application termination pending while active local text generation, Whisper transcription, or model preparation is cancelled and joined. The llama.cpp session and Whisper engine are released before AppKit allows Sparkle to relaunch the application, preventing process-global Metal cleanup from encountering live model resources.

The same deterministic cleanup applies to ordinary Quit. Notes are flushed first, active-dictation quit choices remain unchanged, and no note content is transmitted or modified by this lifecycle fix.

Compatibility: macOS 14 or later.
