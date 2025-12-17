# Quality Gates Demo

This repository demonstrates how to set up **quality gates** in a JavaScript project using **Prettier** and **ESLint**, enforced via **GitHub Actions**.

## 🚦 Quality Gates

The project includes a CI workflow that runs on every push and pull request to ensure code quality before any further steps (such as UI or API tests).

The quality gate consists of:

- **Prettier** — checks code formatting
- **ESLint** — checks code quality and potential errors

If any formatting or linting issue is detected, the pipeline fails early and blocks the pull request.

## 📦 Available Scripts

```bash
npm run format        # Check formatting with Prettier
npm run format:write  # Automatically fix formatting issues
npm run lint          # Run ESLint
npm run lint:fix      # Automatically fix lint issues

⚙️ CI Workflow
The GitHub Actions workflow is defined in:
.github/workflows/quality-gates.yml. -> It installs dependencies and runs Prettier and ESLint as a quality gate.

🛠 Tech Stack
    - Node.js 20
    - Prettier
    - ESLint (flat config)
    - GitHub Actions

```
