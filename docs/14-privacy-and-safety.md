# Privacy and safety

## Purpose
This document defines the privacy and safety posture for Starlight and clarifies the boundaries of the research platform.

## Background
An always-available assistant raises serious questions about data capture, consent, and trust. The system should be designed so that privacy is not an afterthought. This document is central to the Today and Research layers because a prototype will only gain user trust if it is explicit, configurable, and conservative about data handling.

## Goals
- Preserve user trust through clear controls and transparent defaults.
- Limit unnecessary capture and retention.
- Support safety in contexts where the assistant prompts, navigates, or reminds the user.

## System design
The privacy model should include:
- Explicit consent for sensitive capture and data retention.
- Clear controls for what is stored, shared, and deleted.
- Graceful fallbacks when sensors or network access are unavailable.
- Strong separation between personal context and broader system telemetry.

## Key workflows
- Review and delete stored notes or captured context.
- Choose which devices should receive reminders or summaries.
- Disable any feature that is not desired in a given moment.

## Constraints
- Privacy and utility often trade off, so the system should make these tradeoffs visible.
- Some use cases require stronger safeguards than others.
- The system should not imply direct access to private data beyond what the user has explicitly approved.

## Future work
Future work should formalize privacy evaluation metrics, safety testing, and user-facing controls for retention and sharing.

## References
- Privacy engineering and data minimization research.
- Human-centered AI safety and trust literature.
- Accessible and inclusive privacy design guidance.
