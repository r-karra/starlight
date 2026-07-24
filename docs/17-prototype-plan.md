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

## System design
A practical prototype should include:
- Devices: Google XR smart glasses, Android phone, Googlebook or Windows/Linux/Mac laptop, and wearable sensors as supporting surfaces.
- Software and infrastructure: existing developer and research platforms, cloud services, and tools from the broader AI ecosystem.
- AI stack: a primary focus on Gemini/Gemma, with supporting models such as Essential AI's Rn-1 and other companion systems.
- An XR-enabled capture path for quickly recording lectures, notes, and context during learning sessions.
- A companion mobile workflow for reminders, task creation, context syncing, and privacy controls.
- A laptop workflow for deeper review, research, note refinement, and writing.
- A lightweight sync layer that preserves continuity without imposing intrusive attention demands.

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

## Future work
Future iterations can add stronger memory, richer personalization, and more capable multimodal workflows as the prototype matures. A longer-term research path can also explore AOSP-based customization for XR and Android experiences.

## References
- Mobile companion app and cross-device UX practices.
- Early-stage prototyping and usability validation guidance.
- Research methods for human-centered AI experiments.
