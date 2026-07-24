# Repository Guidance

## Project stage

This repository is in Phase 1. Prefer research spikes, explicit documentation, and small reversible changes until the browser client, gateway, asset pipeline, and rAthena integration choices are recorded.

## Working rules

- Keep upstream source history and licensing traceable.
- Do not commit game assets, credentials, production data, or database dumps.
- Do not couple browser code directly to the rAthena database.
- Add setup instructions with environment-changing work.
- Consider desktop and mobile browser behavior for UI changes.
- Record cross-component architectural decisions under `docs/decisions/`.
- Use focused branches and draft pull requests for incomplete work.

## Verification

Include exact commands and manual verification steps in each pull request. Add automated checks only after the relevant language and build stack are selected.
