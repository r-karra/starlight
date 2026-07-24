# Navigation mode

## Purpose
This document describes a navigation-focused mode for Starlight that supports reminders, wayfinding, summarization, and situational awareness.

## Background
Navigation is one of the clearest near-term uses for ambient assistance. It combines agenda context, current location, and short-term memory in a way that benefits from glasses and phone coordination. This mode is well-suited to the Today layer because it provides immediate utility with limited complexity, while also informing later Research and Vision work on richer spatial context and more adaptive assistance.

## Goals
- Support turn-by-turn guidance and situational awareness.
- Reduce cognitive load during travel, unfamiliar routes, or crowded environments.
- Connect navigation to reminders, tasks, and handoff needs.

## System design
The navigation mode should integrate navigation services with task and reminder context:
- Provide lightweight direction or route updates through the glasses or phone.
- Surface relevant reminders at the right time and location.
- Summarize nearby context when helpful, without overwhelming the user.

## Key workflows
- Receive a reminder to pick up a package as you approach the destination.
- Ask for a concise overview of the route or the next step.
- Continue a task after arriving without losing the thread of the earlier context.

## Constraints
- Navigation should not become visually or audibly distracting.
- The system must be robust when connectivity, GPS, or sensor data is imperfect.
- The user should always retain control over what is surfaced.

## Future work
Future work should explore better context-aware routing, more natural handoff to indoor navigation, and richer support for accessibility needs.

## References
- Human factors research on navigation assistance.
- Adaptive mobile guidance and context-aware systems.
- Accessibility and wayfinding studies.
