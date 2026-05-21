# Architecture Rules

## Scope
Applies to repository layout, dependency manifests, and structural changes in this repository.

## Standards
- Keep these top-level directories present for application work: src, tests, config, scripts, docs.
- Before adding runtime code, create and commit the dependency manifest for the selected runtime (for example package.json for Node.js).
- Store environment values in .env and keep only templates in .env.example.
- Structural changes must be split into a dedicated commit when they create, delete, or rename two or more top-level directories.

## Workflow Checks
- If a pull request adds code under src, verify a dependency manifest exists in the repository root.
- If a pull request adds a new top-level directory, update docs or .agents/rules/README.md to describe its purpose.
- If a pull request modifies repository structure, include a short justification in the pull request description.

## Rationale
A stable architecture reduces onboarding friction, prevents ad-hoc folder sprawl, and lowers long-term maintenance risk.