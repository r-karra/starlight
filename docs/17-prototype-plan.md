# Prototype plan

## Purpose
This document outlines a practical prototype plan for Starlight Platform that begins on existing devices and focuses on immediate user value.

## Background
The platform should not begin with a full custom stack. Instead, it should validate the interaction model with a modest prototype that can be built and tested quickly. The prototype should be framed as a cross-device ambient intelligence system where XR glasses coordinate with Android mobile and laptop to reduce cognitive load, support learning, manage tasks, assist navigation, and provide optional reflection support.

The immediate prototype path is grounded in existing hardware and software ecosystems, while a later research direction may explore deeper customization of XR and Android experiences through AOSP-based work.

## Goals
- Prove that reminders, summaries, navigation, study capture, and handoff can work across existing devices.
- Establish a reusable documentation and research foundation for future work.
- Keep the prototype path aligned with the Today layer of the roadmap.
- Explore whether the platform can help reduce screen addiction, technological dependency, work stress, desire-driven stress, and financial anxiety.
- Support an experience that encourages peaceful living, stronger family and social ties, and values-based reflection.

## Success metrics
- reduction in perceived screen and notification overload for prototype users.
- lower education-related or job-related stress in targeted use cases.
- improved continuity of tasks across XR glasses, phone, laptop, and cloud.
- faster concept comprehension and study effectiveness for students.
- higher user trust in privacy, control, and non-intrusive assistance.

## Why this prototype is a good starting point
This prototype focuses on a minimal, testable set of cross-device workflows that align with your mission: reducing addiction, supporting learning, and creating calm, values-aligned support.

It is a good starting point because it:
- uses existing device capabilities rather than assuming platform-level changes,
- builds a clear, measurable path from capture to summary to review,
- keeps privacy and consent explicit,
- leaves deeper OS/AOSP customization as a future research direction.

## System design
A practical prototype should include:
- Devices: Google XR smart glasses, Android phone, Googlebook or Windows/Linux/Mac laptop, and wearable sensors as supporting surfaces.
- Software and infrastructure: existing developer and research platforms, cloud services, and tools from the broader AI ecosystem.
- AI stack: a primary focus on Gemini/Gemma, with supporting models such as Essential AI's Rn-1 and other companion systems.
- An XR-enabled capture path for quickly recording lectures, notes, and context during learning sessions.
- A companion mobile workflow for reminders, task creation, context syncing, and privacy controls.
- A laptop workflow for deeper review, research, note refinement, and writing.
- A lightweight sync layer that preserves continuity without imposing intrusive attention demands.

## MVP scope
The first build should validate a small set of end-to-end workflows with existing hardware and APIs.
- Student workflow: capture lecture audio or notes on XR glasses, generate a study summary, and create tasks or reminders on the mobile companion.
- Research workflow: ask the glasses for topic refinement, route the request through phone/cloud AI services, and present a concise explanation back on the glasses.
- Work workflow: create a project task from voice input, sync it to phone and laptop, and resume deeper work on the laptop later.
- Privacy workflow: allow users to explicitly approve capture, sharing, and device handoff for each session.

## Technical architecture
A minimal architecture should map device roles and data flow clearly:
- Capture layer: XR glasses provide audio, camera, and command capture; the phone provides local user interaction and permissions.
- Orchestration layer: the Android companion app manages context, syncs state, and decides when to route work to laptop or cloud.
- Compute layer: cloud services and AI integrations refine captured content, summarize concepts, and support research assistance.
- Continuity layer: a shared state store keeps tasks, notes, reminders, and selected context available across devices.
- Privacy layer: explicit consent, selective sync, and user review are baked into handoff rules.

## Prototype artifacts
The implementation should produce a small set of artifacts that make the prototype buildable and testable:
- A simplified interaction flow for XR capture → mobile sync → laptop review.
- Wireframes or diagrams for the student capture and research assistance workflows.
- A model integration plan describing which AI services handle summary, topic refinement, and personalization.
- A user validation checklist for stress reduction, continuity, and non-intrusive behavior.

## Aim / Mission
The prototype is intended to bring devices, software stacks, and AI together in a coherent system that helps people reclaim attention from addictive screens and the pressure of constant technology use.

It should prioritize:
- reducing dependency on endless notifications and distracting interfaces,
- easing the stress of work, education, and desire-driven goals,
- supporting a calmer, more grounded life connected to family, community, nature, and faith,
- enabling people to focus on what matters rather than being consumed by what they can wear, eat, or buy.

The broader mission is to create a unified direction that supports peaceful living and encourages a healthy relationship with life priorities in the spirit of the values people find meaningful.

## Use cases
- Infants: keep the environment calm and uncomplicated. The system should not add cognitive burden for caregivers or the child.
- Children and teens: reduce education-related stress, help students understand concepts more intuitively, and provide learning support that aligns with family, society, nature, and faith.
- Mid-age people and job holders: help people get work done, manage projects, and stay organized while avoiding overwhelm and excessive screen dependency.

## Prototype capability: student-oriented orchestration

The prototype will support workflows such as:
- Using Google XR smart glasses to record lectures, capture images, and create note summaries in real time.
- Sending captured context to mobile, laptop, and cloud services so models can refine understanding and personalize teaching support.
- Converting voice or command-based inputs on XR glasses into calendar events, tasks, and reminders that are synchronized with the student's phone and laptop.
- Allowing the student to ask the glasses for research help, then coordinating across devices and AI services to gather refined content, explain concepts, and support exploration.
- Delivering results through speaker and display on the glass device while preserving the ability to continue work on the phone or laptop later.

These workflows should remain explicit, permission-driven, and oriented toward lowering stress and freeing time for personal relationships and reflection.

## Key workflows
- Create a reminder from a voice or text prompt.
- Capture a short note or lecture fragment and receive a summary.
- Continue the task later on the laptop with the same context.
- Orchestrate research support across XR glasses, phone, laptop, and cloud services.

## Constraints
- The prototype should remain modest and testable.
- It should prioritize cross-device flow and user trust over feature breadth.
- It should avoid implying that proprietary internals can be changed directly.
- It should clearly separate immediate companion app work from later AOSP-based OS research.

## Implementation roadmap
A phased prototype roadmap helps keep the work grounded and testable.

### Phase 1: Companion workflows and capture
- Build an XR-enabled lecture capture and note summary workflow using existing smart glasses and mobile input.
- Create a mobile companion experience for reminders, task creation, and privacy control.
- Sync captured context with a lightweight cloud state store so phone and laptop continuity can be demonstrated.
- Validate the student workflow with lecture capture, note generation, and calendar/task creation.

### Phase 2: Cross-device handoff and research support
- Add explicit orchestration patterns for handoff between glasses, phone, laptop, and cloud.
- Implement simple research assistance that uses captured context to refine search or study results.
- Demonstrate a student asking XR glasses for topic explanation and receiving follow-up content through the device.
- Add support for job-holder workflows, such as task progress tracking across devices and low-friction work reminders.

### Phase 3: Stress reduction and values-oriented support
- Introduce prototype features that help users reduce screen and notification overload.
- Add contextual reflection prompts and calm reminders that encourage family, society, nature, and faith-centered priorities.
- Validate whether the prototype measurably reduces perceived stress and supports more peaceful daily rhythms.

### Phase 4: Research and longer-term OS direction
- Explore AOSP-based prototyping only once the core interaction model is validated.
- Investigate whether deeper platform customization can improve XR capture, task routing, and privacy controls.
- Use prototype results to guide research on trust, continuity, multimodal context, and adaptive assistance.

## Future work
Future iterations can add stronger memory, richer personalization, and more capable multimodal workflows as the prototype matures. A longer-term research path can also explore AOSP-based customization for XR and Android experiences.

## References
- Mobile companion app and cross-device UX practices.
- Early-stage prototyping and usability validation guidance.
- Research methods for human-centered AI experiments.
