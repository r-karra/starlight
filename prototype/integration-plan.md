# Integration plan

## Purpose
Describe the concrete APIs, services, and integration points for the Starlight prototype.

## XR capture
- target XR device: Google XR-compatible smart glasses or supported headset
- capture inputs: audio, voice/command, images
- SDKs/APIs: use the device’s existing developer SDK for capture and display
- output: captured audio/text and a simple intent payload

## Android companion
- app responsibilities:
  - receive capture payloads from XR glasses
  - manage user consent and privacy settings
  - create tasks, reminders, and notes
  - sync selected context to the cloud and laptop
- integration points:
  - local device communication (Bluetooth, Wi-Fi, or companion SDK)
  - REST or websocket backend for sync
  - local storage for pending actions and user preferences

## Cloud/backend
- responsibilities:
  - store selected task/context state
  - route AI requests and return results
  - provide a sync endpoint for phone and laptop
- minimal backend APIs:
  - `POST /capture` — receive captured context
  - `POST /ai/process` — summarize or refine content
  - `GET /sync` — retrieve synced state for laptop
  - `POST /task` — create or update tasks/reminders

## AI integration
- primary model: Gemini/Gemma (or equivalent reasoning/summarization API)
- support models:
  - transcription model for audio capture
  - task extraction model for reminders
  - knowledge/refinement model for research requests
- integration pattern:
  - capture -> transcription -> summarization/refinement -> task extraction
  - keep AI output limited to concise summaries and follow-up suggestions

## Laptop review interface
- responsibilities:
  - show synced notes, summaries, and tasks
  - enable deeper review and editing
- integration points:
  - sync API from cloud/backend
  - optional web interface or desktop app
  - minimal UI for review and follow-up action

## Privacy and consent
- explicit consent before processing any capture
- selective sync: only approved items move to the cloud or laptop
- clear user control over what is shared across devices
- minimal retention of sensitive session data
