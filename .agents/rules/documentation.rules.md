# Documentation Rules

## Scope
Applies to project-level docs, contribution guidance, and operational notes.

## Standards
- Keep README split between Current Status and Planned Features so readers can distinguish implemented work from roadmap items.
- When adding runtime tooling, include Setup and Run sections in README in the same pull request.
- When collaboration starts (first external contributor or first pull request review), add CONTRIBUTING with branch, commit, and review workflow.
- Any pull request that changes behavior, commands, or structure must update related docs in the same change set.

## Workflow Checks
- If a pull request adds a new command, verify README includes where and how to run it.
- If a pull request adds or renames top-level folders, verify docs mention their purpose.
- If documentation is intentionally deferred, add a Deferred Docs note in the pull request description with owner and due phase.

## Rationale
Accurate documentation reduces setup errors, misalignment, and handoff risk.