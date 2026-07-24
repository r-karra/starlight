# Hardware architecture

## Purpose
This document explains the hardware roles within the Starlight ambient intelligence platform and the rationale for a phased deployment strategy. The repository and platform are named Starlight; "Project Divine Connect" remains the working codename for the first product concept.

## Background
The system is organized as a device ecology rather than a single product. That structure allows the research effort to begin with existing hardware while preserving a path toward more specialized reference hardware.

## Goals
- Clarify the role of XR smart glasses, Android mobile devices, laptop workstations, and cloud infrastructure.
- Preserve a path from current devices to reference hardware.
- Keep the roadmap grounded in near-term feasibility rather than speculative product claims.

## System design
- Smart glasses: primary human interface for glanceable prompts, lightweight assistance, and hands-free input.
- Android phone: coordination and execution hub for reminders, context handling, and app orchestration.
- Laptop workstation: knowledge work surface for longer writing, analysis, and structured tasks.
- Cloud: synchronization, storage, backup, and cross-device continuity.

The design should not assume that custom hardware is immediately available. Instead, the system should first demonstrate value on currently available devices and only then define a reference hardware target for future work.

## Key workflows
- The glasses present a short summary or reminder while the user is moving.
- The phone resolves the action, potentially by launching a companion workflow or task.
- The laptop handles a more complex request that benefits from a larger interface and richer editing surface.

## Constraints
- Wearable hardware may have limited compute, battery, and thermal headroom.
- Audio and visual privacy remain essential design concerns.
- Cross-device compatibility must be preserved across a range of hardware generations.

## Future work
The mid- to long-term hardware agenda should define reference hardware for glasses, phone, and laptop, including sensor placement, display characteristics, and modularity for future experiments.

## References
- XR hardware design references and human factors studies.
- Mobile device platform capabilities and sensor tradeoffs.
- Wearable computing research on thermal, power, and interaction constraints.
