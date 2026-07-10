# Agentic Product Development Project

Follow `METHODOLOGY.md` and begin every task by reading `docs/status/product-status.md`.

## Working model

- Develop a validated MVP first, then evolve the product through explicit version specifications.
- Use the orchestrator as the default user-facing role.
- Delegate only bounded work that benefits from isolated context, specialized tools or independent review.
- Use the matching question bank under `question-banks/` for each role.
- Ask one to five related questions per turn and close by exit criteria.
- Invoke `create-guided-questionnaire` when more than 12 relevant questions remain, multiple participants must answer or the user requests offline completion.
- Load only selected domain and technical packs from `knowledge-packs/`.
- Treat catalog capabilities as hypotheses until the user approves them.
- Keep `docs/status/product-status.md` current and concise.

## Documentation map

- `docs/product/product-overview.md`: cross-functional product view.
- `docs/product/mvp-scope.md`: approved MVP boundary.
- `docs/versions/`: changes and releases.
- `docs/ux/`: journeys and UX/UI guidance.
- `docs/architecture/`: architecture and ADRs.
- `docs/engineering/`: implementation contracts and designs.
- `docs/quality/`: test strategy and release evidence.
- `docs/operations/`: deployment, observability and runbooks.

## Boundaries

- Never invent stakeholder answers or hide uncertainty.
- Never expand MVP scope without explicit approval.
- Ask before changing public contracts, schemas, dependencies, production data or external systems.
- Never commit secrets.
- Use read-only subagents for independent review when possible.
- Do not run concurrent edits on the same files.

## Completion

Work is complete only when acceptance, verification, documentation, deployment/rollback and QA release-gate requirements applicable to the change are satisfied.

