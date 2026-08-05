# Initial Architecture

This document captures the working boundaries for Phase 1. It is intentionally technology-neutral until the technical spikes are complete.

## System boundaries

| Component | Responsibility | Phase 1 status |
| --- | --- | --- |
| Web launcher | Server status, news, download-free launch flow, responsive account UI | Design and spike |
| Browser client adapter | Isolate roBrowser integration and browser compatibility fixes | Research |
| Gateway API | Keep browser-facing APIs separate from emulator internals | Design |
| rAthena | Authentication, character, map, and game-server behavior | Upstream dependency |
| Asset pipeline | Convert, version, validate, and serve client assets legally | Research |
| Operations | Local containers, Ubuntu 26 deployment, logs, backups | Design |

## Proposed request flow

1. The player opens the launcher.
2. The launcher requests public status and configuration from the gateway.
3. Authentication is handled through a dedicated web-facing endpoint.
4. The browser client receives a short-lived session rather than database credentials.
5. The client connects through the protocol adapter to the emulator services.
6. Static assets are served from a versioned asset origin.

## Security boundaries

- Do not expose the rAthena database directly to browsers.
- Do not store plaintext passwords, access tokens, or production secrets in Git.
- Treat imported client assets as untrusted input during conversion.
- Use separate development, staging, and production configuration.
- Define rate limiting, session expiry, CSRF protection, and audit logging before public registration.

## Technical decisions still open

- roBrowser fork versus compatibility layer
- WebSocket/TCP bridge design
- Launcher framework and build tool
- Gateway language and framework
- Asset conversion and patching strategy
- rAthena packet version and client compatibility target
- Database ownership for web accounts
- Deployment topology and CDN choice

Decisions that affect more than one component should be recorded as Architecture Decision Records under `docs/decisions/`.
