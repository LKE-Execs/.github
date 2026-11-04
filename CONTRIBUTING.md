# Contributing to LKE Inc Repositories

Welcome to the team! This guide applies to everyone: employees and interns.

---

## 1. Security & Core Principles
1. **Never commit secrets:** Never commit passwords, tokens, API keys, or `.env` files. If you do by accident, notify a senior team member immediately so the secret can be rotated.
2. **Never push directly to `main`:** All work happens on feature branches and goes through Pull Request (PR) review.
3. **Keep PRs small:** PRs under 300 lines are reviewed and merged much faster.

---

## 2. Branch Naming
Create branches using this format:
```
<type>/<short-description>
```

Types:
- `feat/` — New feature or capability
- `fix/` — Bug fix or error resolution
- `chore/` — Dependency updates, build configs, tool setup
- `docs/` — Documentation updates only
- `refactor/` — Code reorganization with no behavior change
- `test/` — Adding or modifying tests

*Example:* `feat/customer-metrics-dashboard` or `fix/pipeline-null-error`

---

## 3. Commit Message Standards (Conventional Commits)
Format:
```
<type>: <imperative description in lowercase>
```

Examples:
- `feat: add user filter dropdown on dashboard`
- `fix: resolve divide-by-zero error in pipeline calculations`
- `docs: update setup instructions in readme`
- `chore: bump dependencies in package.json`

---

## 4. Development Workflow
1. Pull latest `main`: `git checkout main && git pull`
2. Create branch: `git checkout -b feat/your-feature-name`
3. Develop locally (with Claude Code) and test your changes
4. Check status: `git status`
5. Commit: `git add <files>` then `git commit -m "feat: description"`
6. Push: `git push -u origin feat/your-feature-name`
7. Open Pull Request on GitHub and request review from `@lke-inc/employees`
8. At least 1 employee approval is required before merging
