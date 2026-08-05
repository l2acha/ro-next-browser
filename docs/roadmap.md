# Roadmap

## Phase 1 — Modern RO Browser foundation

Goal: prove that a maintainable browser client can connect to a controlled rAthena environment.

### Workstreams

- Audit roBrowser structure, dependencies, build process, and browser APIs.
- Audit rAthena setup, packet version, database schema, and login flow.
- Create a reproducible Ubuntu 26 development environment.
- Establish the smallest playable connection between roBrowser and rAthena.
- Document asset requirements and licensing constraints.
- Design a responsive launcher and account flow.
- Add basic linting, tests, and continuous integration after the stack is selected.

### Exit criteria

- A new developer can reproduce the environment from documentation.
- The browser client reaches login, character selection, and a test map.
- Known compatibility failures are tracked as issues.
- No credentials or unlicensed distributable assets are committed.
- The launcher architecture and Phase 2 backlog are approved.

## Phase 2 — Product foundation

- Web registration and account recovery
- Server status, announcements, and patch metadata
- Mobile-first controls and responsive game viewport
- Containerized staging deployment
- Logging, metrics, rate limits, and backups
- Automated browser compatibility tests

## Phase 3 — Cloud and AI capabilities

- Web administration portal
- AI-assisted support, documentation, and operations
- Player-facing guide and quest assistant
- Multi-server orchestration
- Progressive Web App packaging
- Controlled mobile distribution strategy

Phase 3 AI features must not automate unfair gameplay or bypass server rules.
