# Repository structure

## Purpose
This document suggests a practical code repository structure for the Starlight prototype.

## Recommended structure
- `mobile/` — Android companion app source and mobile integration code
- `xr/` — XR device capture app or SDK integration code
- `backend/` — lightweight backend for sync, AI orchestration, and data storage
- `laptop/` — web or desktop review interface source code
- `prototype/` — documentation, build plans, tasks, and validation artifacts
- `docs/` — architecture, research, and product definition documents

## Notes
- Keep the prototype code structured so each device surface has a clear boundary.
- The backend should remain minimal and API-driven.
- If the laptop interface is a web app, it can be hosted in `laptop/` or merged with `backend/` depending on the stack.
- Keep documentation in `prototype/` and `docs/` separate from implementation code.
