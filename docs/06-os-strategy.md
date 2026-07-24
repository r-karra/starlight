# OS strategy

## Purpose
This document frames the operating system strategy for Starlight Platform as a future direction rather than an immediate implementation claim.

## Background
The platform is intentionally described as compatible with existing devices first. A deeper customization path can later be considered through Android Open Source Project (AOSP)-based work, especially for XR smart glasses and Android mobile experiences that may benefit from more explicit control of capture, task routing, and privacy.

## Goals
- Avoid making unsupported claims about proprietary platform internals.
- Position AOSP-based customization as a long-term, research-oriented direction.
- Provide a realistic path from prototype to deeper integration.
- Preserve a clear distinction between current companion-app prototypes and later OS-level research work.

## System design
The proposed strategy has three stages:
1. Prototype on existing Android and XR-capable platforms using companion applications and current APIs.
2. Validate interaction models, privacy controls, and orchestration patterns on off-the-shelf hardware.
3. Explore AOSP-based customization only for future reference hardware or open components when the interaction model is mature.

This does not imply that Google or other vendors would directly expose private internals. Instead, the research path should be framed as an ecosystem and platform exploration that could eventually use AOSP-based components where appropriate.

## OS responsibilities
- A prototype can run using current device capabilities and existing app infrastructure.
- A later OS layer could improve system-level handoff, background coordination, and device-specific behaviors.
- The user should remain able to control permissions, defaults, and privacy boundaries.

## Constraints
- Platform restrictions on current devices may limit the depth of integration.
- An AOSP-based path requires substantial engineering and validation.
- The system’s value should be demonstrated before deeper customization is pursued.

## Future work
Future work should evaluate the feasibility of a modular OS layer for gesture handling, task routing, audio prompts, and cross-device trust policies.

## References
- AOSP architecture and platform customization documentation.
- Android device integration and companion app patterns.
- Research on secure and privacy-preserving OS-level services.
