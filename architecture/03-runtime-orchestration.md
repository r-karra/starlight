# Runtime orchestration architecture

## Purpose

This document specifies the subsystem responsible for coordinating activity across devices and services. It governs how tasks are routed, scheduled, and handed off without requiring the user to manually manage each step.

## Responsibilities

The runtime orchestration layer decides which subsystem or device should handle a task given available context, user preferences, and system constraints. It provides the control plane for the platform’s distributed behavior.

## Core components

- Task router: classifies intents and selects the most appropriate execution path.
- Device coordinator: manages handoffs between glasses, mobile, laptop, and cloud services.
- Policy engine: enforces user preferences, safety boundaries, and permission rules.
- Execution broker: submits work to the appropriate runtime endpoint.

## Control model

Orchestration is event-driven and context-sensitive. The system evaluates available signals such as urgency, device capability, user location, and permission state before selecting a target execution path. This supports both immediate assistance and deferred continuation without forcing the user to manage each transition manually.

## State handling

The orchestration layer maintains a task state model that captures intent, progress, handoff state, and completion status. The state model is designed to allow partial execution, asynchronous continuation, and later resumption on another device.

## Failure and recovery

When a task cannot be completed on the current device, the orchestrator should defer it, re-route it, or prompt the user for confirmation rather than fail silently. This preserves continuity and provides a clear path for recovery.

```mermaid
sequenceDiagram
    participant U as User
    participant I as Interaction Layer
    participant O as Orchestrator
    participant E as Execution Layer
    participant C as Cloud Layer

    U->>I: issue intent
    I->>O: forward context
    O->>E: route task
    E->>C: persist state
    C-->>O: acknowledge
    O-->>I: return result
