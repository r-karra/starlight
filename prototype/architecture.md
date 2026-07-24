# Architecture

## Purpose
This document describes the minimal architecture for the Starlight prototype and the relationships between devices, services, and AI.

## Device roles
- XR glasses: primary capture and glanceable interaction surface. They record audio, images, and voice/command input, and deliver succinct responses.
- Android phone: companion orchestrator, local privacy control, task manager, and sync coordinator.
- Laptop: deeper review, research, drafting, and longer-form work.
- Wearables: optional sensors for context, wellbeing, and low-friction state signals.

## System layers
- Capture layer: XR glasses plus mobile capture input. This layer collects the user’s current context and intent.
- Orchestration layer: the Android companion app manages state, coordinates handoff, and decides where tasks should run next.
- Compute layer: cloud services and AI integrations perform summarization, topic refinement, and research assistance.
- Continuity layer: a shared task and context store keeps selected state available across devices.
- Privacy layer: explicit consent, selective sync, and user review are enforced at each handoff.

## Data flow
- The glasses capture a lecture, command, or research request.
- The phone receives the capture, applies privacy rules, and forwards selected context to the cloud.
- The cloud or AI service refines content, creates summaries, and returns actionable results.
- The phone delivers concise follow-up to the glasses and syncs a richer context to the laptop.

## AI integration
- Primary AI: Gemini/Gemma for reasoning, summarization, and concept refinement.
- Support models: Essential AI’s Rn-1 and other companion systems for specialized tasks.
- Use case-specific AI: summarization for lecture capture, question-answering for research support, and task extraction for reminders.

## Practical constraints
- The architecture should remain realizable with current XR and mobile APIs.
- It should avoid assumptions about proprietary OS internals.
- AOSP-based platform work should be treated as a future research extension, not a first-phase requirement.