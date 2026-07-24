# Device orchestration

## Purpose
This document describes how Starlight Platform should coordinate activity across glasses, phone, laptop, and cloud so the experience feels continuous and low-friction.

## Background
Cross-device orchestration is one of the core differentiators of the platform. A useful assistant must know when to respond on the glasses, when to defer to the phone, and when to escalate to the laptop. This capability is foundational for the Today layer, where a prototype must feel coherent across devices, and it becomes more sophisticated as the Research and Vision layers mature.

## Goals
- Define handoff patterns for reminders, summaries, drafting, and task execution.
- Show how context can flow across devices without forcing the user to re-enter information.
- Keep the experience calm and predictable.

## System design
The orchestration model should be event-driven and context-aware across devices and services:
- Devices: Google XR smart glasses capture glanceable prompts, audio, images, and commands.
- Mobile: Android phones coordinate context, privacy controls, reminders, and short-form interactions.
- Laptop: Googlebook or Windows/Linux/Mac laptops handle deeper drafting, review, research, and long-form work.
- Cloud: sync, continuity, AI refinement, and shared state storage support cross-device handoff.

The orchestration model should also integrate AI stack services such as Gemini/Gemma and companion models to refine captured concepts, summarize learning material, and support intuitive research assistance.

- Immediate needs: glasses and phone handle short prompts, reminders, capture, and quick summaries.
- Deeper work: laptop handles drafting, analysis, research, and longer editing.
- Sync and continuity: cloud stores task state, selected context, and refinement results for later retrieval.

The design treats handoff as a first-class architectural concern rather than an application-level convenience. The goal is to maintain continuity of task state across devices while preserving user control over what is shared, delayed, or suppressed.

```mermaid
sequenceDiagram
    participant G as Glasses
    participant P as Phone
    participant L as Laptop
    participant C as Cloud
    G->>P: Intent or prompt
    P->>C: Save context and task state
    P->>L: Escalate when needed
    L->>C: Publish result
    C->>P: Sync response
    P->>G: Deliver concise follow-up
```

## Key workflows
- A reminder created on the phone becomes visible on the glasses at the appropriate moment.
- A note captured during a walk can later become a richer draft on the laptop.
- A study task started on the phone can be resumed on the laptop without losing state.
- A student can ask XR glasses for research help and the system can coordinate context across phone, laptop, cloud, and AI services to refine a concept and explain it back through the glasses.
- A job holder can begin a task on the phone or glasses, let the platform manage scheduling and progress, and complete deeper work on the laptop with continuity.

## Constraints
- Network quality and device availability affect orchestration.
- Hand-off rules should be explainable and controllable by the user.
- Some contexts should not be automatically shared across devices without consent.

## Future work
Future work should define the task state model, context retention policy, and adaptive routing logic for different situations.

## References
- Cross-device UX and continuity research.
- Task handoff and context management studies.
- Mobile and wearable orchestration frameworks.
