# Testing Rules

## Scope
Applies to new features, bug fixes, and refactors once implementation code exists under src.

## Standards
- Each feature or bug-fix pull request that changes src must include at least one automated test in tests.
- Test names must state expected behavior, for example returns error on missing account id.
- Do not merge when test commands fail locally or in CI.
- Avoid non-deterministic tests (time-based sleeps, random seeds without control, external network dependencies).

## Phase Gate
- Current repository state: bootstrap. Until runtime tooling exists, this rule is validated by maintaining the tests directory and documenting planned test command.

## Workflow Checks
- If files in src change and tests do not, the pull request must include a justification section named Test Exception.
- When introducing runtime tooling, add a documented test command to README and use it consistently.

## Rationale
Testing guards against regressions and provides confidence for iterative delivery.