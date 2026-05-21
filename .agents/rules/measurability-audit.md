# Rule Measurability Audit

This audit verifies that standards are testable with observable repository evidence.

## Scoring
- Measurable: can be passed or failed from files, commit metadata, or pull request metadata.
- Conditional measurable: measurable once runtime tooling exists.

## Architecture
- Status: Measurable.
- Evidence points:
  - Top-level directories exist: src, tests, config, scripts, docs.
  - Dependency manifest existence check once runtime code appears under src.
  - Structural commit split trigger defined as two or more top-level directory create/delete/rename operations.

## Naming
- Status: Measurable.
- Evidence points:
  - Branch pattern required: prefix/short-kebab-summary.
  - Branch summary requires at least two hyphen-separated words.
  - Single-word generic commit subjects explicitly rejected.

## Testing
- Status: Conditional measurable.
- Evidence points:
  - If src changes, tests change or pull request includes Test Exception section.
  - Test command required once runtime tooling is introduced.

## Documentation
- Status: Measurable.
- Evidence points:
  - README must include Current Status and Planned Features split.
  - Command changes require README updates.
  - Deferred docs require explicit pull request note with owner and due phase.

## Developer Experience
- Status: Conditional measurable.
- Evidence points:
  - .env.example synchronization required when env keys change.
  - Tooling introduction must include at least one documented runnable command.
  - If targeted and full-suite validation commands both exist, targeted command runs first.

## Remaining Non-Measurable Items
- None identified in the current rule text.
