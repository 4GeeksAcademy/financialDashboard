# Updated Project Rules

## Architecture
### Good Practices:
- Maintain a clear and scalable folder structure (e.g., `src/`, `tests/`, `config/`).
- Use a dependency management file (e.g., `package.json`) to track and install dependencies.
- Plan the tech stack and document it in the `memory-bank` folder.

### Rules to Address Risks:
- Define the folder structure before adding code.
- Ensure all dependencies are added to `package.json` and avoid hardcoding versions.

## Naming
### Good Practices:
- Use descriptive commit messages.

### Rules to Address Risks:
- Establish branch naming conventions (e.g., `feature/`, `bugfix/`, `hotfix/`).
- Avoid vague commit messages like "update" or "fix".

## Testing
### Good Practices:
- Implement a testing framework (e.g., Jest, Mocha).

### Rules to Address Risks:
- Write at least one test for every new feature or bug fix.
- Ensure all tests pass before merging code into the main branch.

## Documentation
### Good Practices:
- Maintain an up-to-date `README.md` with project details.
- Document rules and guidelines in `.agents/rules.md`.

### Rules to Address Risks:
- Add a `CONTRIBUTING.md` file to guide contributors.
- Include setup instructions in the `README.md`.

## Developer Experience (DX)
### Good Practices:
- Use the `memory-bank` folder to organize project information.

### Rules to Address Risks:
- Set up DX tools like linters (e.g., ESLint) and formatters (e.g., Prettier).
- Provide an `.env.example` file for environment variable setup.