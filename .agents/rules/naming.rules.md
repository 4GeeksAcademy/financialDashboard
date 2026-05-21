# Naming Rules

## Scope
Applies to branches, commits, files, folders, and future code symbols.

## Standards
- Use branch prefixes: feature/, bugfix/, hotfix/, chore/, docs/.
- Branch names must follow prefix/short-kebab-summary, for example feature/initial-api-scaffold.
- Commit messages must follow: <Action> <scope> <intent>, for example Add rules validation report.
- Do not use commit subjects that are only generic words such as update, fix, changes, misc, cleanup.
- File and folder names must be lowercase-kebab-case unless framework conventions require another style.

## Workflow Checks
- Before opening a pull request, confirm the branch name matches prefix/short-kebab-summary.
- Before committing, reject subjects that are a single generic word (update, fix, changes, misc, cleanup).
- Before opening a pull request, ensure the branch summary segment contains at least two hyphen-separated words.
- If a file name is shortened for convenience, rename it to an intent-revealing name in the same change.

## Rationale
Consistent naming improves discoverability, code review speed, and release traceability.