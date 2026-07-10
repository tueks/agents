# Agentic Product Development Project

## Mission

Develop this product through a validated MVP followed by explicit, versioned changes. Keep decisions and project state legible in the repository.

## Start every task

1. Read `METHODOLOGY.md` when the lifecycle or artifact is unclear.
2. Read `docs/status/product-status.md`.
3. Identify the current version, requested outcome and affected role.
4. Reuse approved decisions and selected knowledge packs.
5. Ask only blocking questions; use `create-guided-questionnaire` for extensive discovery.

## Agent ownership

- `product-orchestrator`: primary user interaction and workflow coordination.
- `product-owner`: product definition, MVP, roadmap and acceptance.
- `ux-ui-designer`: journeys, flows, interaction and visual guidance.
- `software-architect`: quality attributes, boundaries and ADRs.
- `backend-engineer`: backend design and implementation guidance.
- `frontend-engineer`: frontend design and implementation guidance.
- `qa-engineer`: risk, test strategy, traceability and release gate.
- `platform-engineer`: environments, CI/CD, observability and deployment.
- `project-documentarian`: transversal overview, indexes and documentation health.
- `requirements-facilitator`: question explanation, natural-language translation and question-bank review.

Delegate only independent work or tasks that benefit from isolated context or read-only review. The orchestrator owns the consolidated user-facing response.

## Questions and scope

- Each role uses its file under `question-banks/`.
- Do not ask every question mechanically.
- Interview in batches of one to five related questions.
- If the user does not understand a question, explain its intent, impact, answer structure and a fictional example before continuing.
- Never mix the user's answer with the agent's example or suggestion.
- Generate DOCX/XLSX when more than 12 relevant questions remain, several people must answer, or the user wants offline completion.
- Close a role only when its exit criteria are satisfied.

## Knowledge packs

- Domain and technical packs live under `knowledge-packs/`.
- Load only selected packs.
- Treat common capabilities as hypotheses, not approved requirements.
- Record selected packs in product status.
- Prefer existing project patterns and current official documentation for version-specific claims.

## Documentation map

- Product overview: `docs/product/product-overview.md`
- MVP scope: `docs/product/mvp-scope.md`
- Versions and changes: `docs/versions/`
- UX/UI: `docs/ux/`
- Architecture and ADRs: `docs/architecture/`
- Engineering: `docs/engineering/`
- Quality: `docs/quality/`
- Operations: `docs/operations/`
- Current state: `docs/status/product-status.md`

Keep this file as a map. Put detailed knowledge in the referenced documents and skills.

## Boundaries

- Never invent stakeholder answers.
- Never expand MVP scope without explicit approval.
- Ask before adding production dependencies, changing public contracts, modifying production data, deploying or performing destructive actions.
- Never expose or commit secrets.
- Use read-only agents for independent review when possible.
- Do not allow two agents to edit the same files concurrently.

## Definition of done

- Acceptance criteria are satisfied.
- Applicable build, tests and checks pass.
- Tests are proportional to risk.
- Architecture boundaries and security controls remain valid.
- Affected documentation and contracts are updated.
- Deployment, observability and rollback are known.
- QA records a release-gate result.
- Product status identifies the next action.
