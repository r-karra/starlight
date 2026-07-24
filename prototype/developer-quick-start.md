# Developer quick start

## Purpose
This guide is a one-page starting point for building the first working Starlight prototype.

## Build objective
Create a small cross-device workflow that validates the core idea:
- XR glasses capture lecture or research intent
- Android companion manages context, consent, and sync
- Laptop provides deeper review and task continuity
- AI services refine captured content and produce summaries or explanations

## Recommended stack
- XR device: existing Google XR-compatible smart glasses or a supported XR development platform
- Mobile: Android companion app
- Laptop: web app or desktop app for review and authoring
- Cloud: lightweight backend for sync and AI orchestration
- AI: Gemini/Gemma or equivalent summarization and reasoning model, with support models for transcription and task extraction

## First prototype workflow
1. Capture lecture audio or a command on XR glasses.
2. Send the captured context to the Android companion.
3. Ask the companion to process the capture with an AI summarization service.
4. Create a study note, calendar event, or reminder on the phone.
5. Sync the note/task to the laptop for later review.

## Minimum features for phase 1
- XR capture input and voice/command recognition
- Android companion UI for consent and task creation
- Basic cloud or local sync service
- AI-powered summary generation
- A simple laptop review page or document view

## Phase 1 implementation checklist
- [ ] Confirm target XR device and available SDKs/APIs
- [ ] Build a minimal Android companion app
- [ ] Set up a lightweight sync backend or local coordination service
- [ ] Integrate a summarization AI API for captured content
- [ ] Validate end-to-end student capture workflow

## Key design principles
- Keep it simple: avoid too many features in the first build
- Prioritize clarity: make capture, consent, and handoff explicit
- Preserve user control: let users approve what is shared
- Focus on calmness: reduce notifications and avoid interruptions
- Validate with real use cases: students, job holders, and mindful reflection

## Next steps after phase 1
- Add explicit cross-device handoff rules (Phase 2)
- Add calm reminders and reflection support (Phase 3)
- Explore deeper OS-level research only after the core flow is validated (Phase 4)

## Reference artifacts
- `prototype/implementation-plan.md`
- `prototype/architecture.md`
- `prototype/user-flows.md`
- `prototype/tech-stack.md`
- `prototype/validation-plan.md`
