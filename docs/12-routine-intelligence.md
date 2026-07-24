# Routine intelligence engine

## Purpose
This document describes the Routine Intelligence Engine, a reusable AI subsystem within the Starlight Platform for wellness, routines, reminders, and healthy habits without presenting itself as a medical system.

## Background
Wellness support is a strong fit for ambient assistance because routines often depend on time, context, and gentle prompting. The system should support healthy habits without making diagnostic or treatment claims. This subsystem is best framed as a flexible support layer for the Today and Research phases, with more advanced personalization possible in later work.

## Goals
- Offer reminders and suggestions for routines, hydration, movement, and rest.
- Support reflection on habits and progress without overstepping into diagnosis.
- Keep wellness features configurable and optional.

## System design
The Routine Intelligence Engine should be designed as a supportive layer:
- Reminders: hydration, medication timing if appropriate for the user’s own setup, stretching, sleep routines, and check-ins.
- Suggestions: lightweight nudges based on schedule and context.
- Tracking: simple logs or progress summaries when the user opts in.

This subsystem is intended to support wellbeing and routine management through optional, configurable assistance.

## Key workflows
- Receive a gentle reminder to hydrate or take a short movement break.
- Review a daily or weekly routine summary.
- Use context-aware prompts to support focus, recovery, and interpersonal timing.

## Constraints
- The system must not present itself as a medical diagnosis tool.
- Health-related suggestions should be clearly framed as support and personal preferences.
- Users should be able to disable or customize wellness features at any time.

## Future work
Future work should study how reminders and suggestions affect wellbeing without becoming intrusive or patronizing.

## References
- Behavioral design and habit formation research.
- Wellness and digital nudging studies.
- Accessibility and inclusive design guidance.
