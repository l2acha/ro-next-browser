# Contributing

## Workflow

1. Create or select an issue before substantial work.
2. Branch from `main` using `feature/<topic>`, `fix/<topic>`, or `chore/<topic>`.
3. Keep changes small and focused.
4. Document setup or behavior changes in the same pull request.
5. Open a draft pull request early for architectural work.
6. Merge only after relevant checks pass and review feedback is resolved.

## Commit guidance

Use short imperative messages, for example:

- `feat: add launcher status card`
- `fix: handle websocket reconnect`
- `docs: record packet version decision`
- `chore: add browser test workflow`

## Security and assets

Never commit credentials, database dumps, production configuration, proprietary game assets, or third-party source without confirming its license and preserving attribution.

## Definition of done

- The requested behavior is implemented.
- Relevant tests or reproducible verification steps are included.
- Mobile and desktop impact is considered.
- Documentation is updated.
- No secrets or restricted assets are present.
