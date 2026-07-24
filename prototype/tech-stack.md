# Tech stack

## Purpose
This document recommends a practical stack for building the Starlight prototype.

## Devices
- XR glasses: an existing Google XR-compatible device or equivalent smart glasses platform.
- Mobile: Android phone running a companion app.
- Laptop: Googlebook, Windows, Linux, or macOS for deeper review and research.
- Wearables: optional sensors for context and wellbeing signals.

## Platforms
- XR platform: existing headset SDKs and APIs for voice, camera, audio, and display.
- Android: companion app for orchestration, permissions, task sync, and local UI.
- Web/desktop: web app or cross-platform desktop app for laptop review.
- Cloud: lightweight backend and sync store.

## AI services
- Gemini/Gemma: primary model for summarization, reasoning, and concept refinement.
- Essential AI’s Rn-1: support model for companion tasks.
- Other models: specialized APIs for transcription, speech recognition, or research retrieval.

## Backend and sync
- Lightweight cloud service: task and context sync, user preferences, and selective state retention.
- Data storage: encrypted notes, tasks, and selected context.
- API layer: support for device upload, AI request orchestration, and cross-device handoff.

## Integration suggestions
- Start with public APIs and existing SDKs rather than custom OS-level integrations.
- Build the mobile companion first as the core orchestrator.
- Use the laptop as the deeper review surface and optional authoring environment.
- Reserve AOSP-based customization for later research once the core workflow is validated.

## Future direction
- Investigate AOSP-based XR and Android customization only after the prototype demonstrates value.
- Keep the architecture modular so platform-specific pieces can evolve without affecting the core experience.