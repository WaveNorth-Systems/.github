# Contributing

Thank you for contributing to a Wave North Systems project.

## Before starting

1. Confirm the expected outcome in an issue or an approved work item.
2. Check the repository README and local contribution instructions.
3. Create a short-lived branch from the repository's active integration branch.
4. Keep credentials, customer data, and production exports out of commits.

## Branches and commits

- Use descriptive branch names such as `feature/customer-import` or `fix/payment-timeout`.
- Keep each pull request focused on one outcome.
- Write commit messages that explain the result of the change.
- Rebase or update the branch before requesting final review when the target branch has moved.

## Pull requests

- Explain the problem and the resulting behavior.
- Include validation steps and screenshots when the interface changes.
- Call out migrations, new environment variables, permissions, or deployment steps.
- Request review from the team responsible for the affected area.
- Resolve review comments and required checks before merge.

## Quality and security

- Add or update meaningful tests for behavior that can regress.
- Run the repository's required checks locally when practical.
- Report vulnerabilities privately according to [SECURITY.md](SECURITY.md).
