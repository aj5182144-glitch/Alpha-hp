# ALPHA AI — Android starter

ALPHA is an early Android assistant prototype built with Kotlin and Jetpack Compose.

Included in v0.1.0:
- Blue holographic-style interface.
- Home, chat, modules and settings tabs.
- Basic local demonstration responses (not a connected AI model).
- Android speech recognition launched only when the user taps the microphone button.
- Android text-to-speech for reading replies.

Not included yet:
- No cloud AI provider is connected.
- No local language model is bundled.
- No autonomous control of other apps or Android settings.
- No app/plugin generator.
- Voice gender depends on voices installed on the Android device; the selector is currently informational.

Build:
The GitHub Actions workflow builds a debug APK on pushes to main or by manual workflow dispatch. Download the artifact named ALPHA-debug-APK from the workflow run.

This is a development APK, not a Play Store release. Review Android permission prompts and install only builds you trust.
