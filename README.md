# RO Next Browser

A modern browser-first Ragnarok Online platform built around **roBrowser** and **rAthena**, with a responsive web launcher and a path toward mobile and cloud deployment.

> Project status: Phase 1 — research, compatibility validation, and architecture setup.

## Vision

RO Next Browser aims to make a Ragnarok Online server accessible from modern browsers and mobile devices while keeping deployment and administration manageable from the web.

## Phase 1 goals

- Analyze the current roBrowser and rAthena codebases.
- Establish a reproducible Ubuntu 26 development environment.
- Connect roBrowser to a local rAthena server.
- Document packet, asset, authentication, and browser compatibility gaps.
- Build a modern responsive launcher foundation.
- Define test and deployment workflows before adding production features.

## Planned repository layout

```text
apps/
  launcher/       Web launcher and account UI
  game-client/    Browser client integration layer
services/
  gateway/        API/authentication boundary
infra/
  docker/         Local and server containers
docs/             Architecture, setup, decisions, and roadmap
```

The application folders will be introduced only after the technical spike selects the framework, asset pipeline, and integration approach.

## Principles

- Keep upstream projects traceable; avoid copying code without preserving license and attribution.
- Never commit game assets, credentials, private server data, or production secrets.
- Prefer reproducible local development and small reviewable changes.
- Validate desktop and mobile browser behavior from the beginning.

## Upstream references

- [roBrowser](https://www.robrowser.com/)
- [rAthena Thailand](https://github.com/rAthena-Thailand/rathena)
- [Hercules](https://github.com/HerculesWS/Hercules)

## Licensing

No project-wide license has been selected yet. Third-party code and assets remain subject to their respective licenses. Complete the licensing and attribution review before importing upstream source or distributing game assets.
