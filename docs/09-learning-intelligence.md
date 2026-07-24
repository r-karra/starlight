# Learning intelligence engine

## Purpose
This document describes the Learning Intelligence Engine, a reusable AI subsystem within the Starlight Platform for lecture capture, study support, and revision planning.

## Background
Students and learners often face a high volume of information and limited time for review. A calm assistive system can turn captured material into structured study support with less manual effort. This subsystem is a strong Today-layer prototype because it offers immediate value through summaries, notes, and revision support, while also generating research questions for personalization and multimodal understanding.

This work is also grounded in a broader mission to reduce screen addiction, relieve education stress, and free time for family, faith, society, and nature.

## Goals
- Support lecture capture and post-class summarization.
- Offer revision planning using weak-topic detection and spaced review.
- Reduce friction between listening, note-taking, and follow-up study.
- Help learners spend less time wrestling with tools and more time understanding ideas and living intentionally.

## System design
The Learning Intelligence Engine should combine capture, summarization, and planning:
- Capture: audio, slides, handwritten notes, or screenshots from class, with support for XR glasses and mobile capture.
- Summarization: generate concise summaries and key takeaways.
- Study support: create flashcards, detect weak topics, and suggest revision blocks.
- Research assistance: use AI models and cloud services to refine concept understanding and help students explore topics more intuitively.
- Handoff: move from glasses or phone capture to laptop review when more depth is needed.

The subsystem should leverage AI stacks such as Gemini/Gemma and supporting companion models to personalize study support and reduce the friction of learning.

This subsystem is designed to operate as a reusable study-support layer rather than a narrow classroom tool.

## Key workflows
- Record a lecture and later retrieve a summary with action items.
- Generate flashcards from key concepts and identify weak topics for revision.
- Build a revision plan that balances upcoming deadlines and prior performance.

## Constraints
- Transcription and extraction quality may vary by environment and speaker.
- Students may need flexible controls for how much content is processed and stored.
- The system should support both quick summaries and deeper study workflows.

## Future work
Future work should evaluate the quality of study recommendations, explore better personalization, and test multimodal capture in classroom environments.

## References
- Learning science and spaced repetition research.
- Lecture capture and note-taking support studies.
- Educational technology and adaptive learning literature.
