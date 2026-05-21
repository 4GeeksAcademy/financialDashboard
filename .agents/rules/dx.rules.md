# Developer Experience Rules

## Scope
Applies to local developer workflows, formatting, linting, and environment setup.

## Standards
- Maintain .env.example with only non-secret keys used by local development.
- Once runtime tooling is introduced, add scripts for lint, format, and test in the project manifest.
- Recurring actions (start, test, lint, format) must be executable by documented commands instead of manual multi-step instructions.
- Run a changed-file or targeted check before full-suite validation when both are available.

## Phase Gate
- Current bootstrap phase requirement: keep .env.example present and synchronized with documented configuration keys.
- First implementation phase requirement: add and document lint, format, and test commands.

## Workflow Checks
- If new env keys are introduced, update .env.example in the same pull request.
- If new tooling is introduced, add at least one documented command that runs it locally.
- If both targeted and full-suite commands exist, run the targeted command first and record failures before running the full suite.

## Rationale
Strong developer experience improves consistency, reduces friction, and shortens cycle time.