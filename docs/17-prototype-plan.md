# Prototype plan

## Purpose
This document outlines a practical prototype plan for Starlight Platform that begins on existing devices and focuses on immediate user value.

## Background
The platform should not begin with a full custom stack. Instead, it should validate the interaction model with a modest prototype that can be built and tested quickly. The prototype should be framed as a cross-device ambient intelligence system where XR glasses coordinate with Android mobile and laptop to reduce cognitive load, support learning, manage tasks, assist navigation, and provide optional reflection support.

## Goals
- Prove that reminders, summaries, navigation, study capture, and handoff can work across existing devices.
- Establish a reusable documentation and research foundation for future work.
- Keep the prototype path aligned with the Today layer of the roadmap.

## System design
A practical prototype should include:
- A mobile companion app or workflow for reminders, summaries, and task creation.
- An XR-capable device path for glanceable prompts and quick capture.
- A laptop workflow for deeper drafting or review.
- A simple sync layer for cross-device continuity.

## Prototype capability: research orchestration

The prototype will support:
- searching trusted research sources
- collecting references
- summarizing papers
- organizing reading lists
- creating study plans
- generating experiment notes
- tracking progress across sessions

These capabilities should remain permission-based and should operate through approved sources, public resources, or authorized integrations rather than assuming unrestricted access.

## Key workflows
- Create a reminder from a voice or text prompt.
- Capture a short note or lecture fragment and receive a summary.
- Continue the task later on the laptop with the same context.

## Constraints
- The prototype should remain modest and testable.
- It should prioritize cross-device flow and user trust over feature breadth.
- It should avoid implying that proprietary internals can be changed directly.

## Future work
Future iterations can add stronger memory, richer personalization, and more capable multimodal workflows as the prototype matures.

## References
- Mobile companion app and cross-device UX practices.
- Early-stage prototyping and usability validation guidance.
- Research methods for human-centered AI experiments.
