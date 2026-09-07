# Repository Standards

Use this checklist when a project is created in or transferred to Wave North Systems.

## Ownership and access

- Keep the repository private unless company leadership approves publication.
- Grant access through a responsible team instead of adding broad direct access.
- Maintain at least two trusted organization owners for recovery coverage.
- Review outside collaborators and inactive access regularly.

## Repository metadata

- Use a clear, stable, lowercase repository name with hyphens.
- Add a concise description, product homepage when available, and relevant topics.
- Keep the default branch named `main` unless a documented migration constraint prevents it.
- Add a README that explains purpose, setup, architecture, validation, deployment, and ownership.

## Change control

- Require pull requests before merging to the default branch.
- Require at least one approving review for normal changes.
- Dismiss stale approvals after material changes.
- Require conversation resolution and the repository's meaningful status checks.
- Block force pushes and branch deletion on protected branches.
- Use a merge queue or stricter review for repositories where concurrent changes create release risk.

## Security

- Enable secret scanning, push protection, Dependabot alerts, and automated security updates where the GitHub plan and repository visibility support them.
- Store secrets in GitHub environments, Railway, Supabase, or another approved secret manager.
- Protect production environments with named reviewers when the plan supports it.
- Keep generated exports, database snapshots, `.env` files, and private keys out of Git.
- Add a `CODEOWNERS` file in each repository based on its actual responsible teams.

## Automation

- Run formatting, linting, tests, builds, and migration validation appropriate to the stack.
- Pin third-party GitHub Actions to reviewed versions and keep them updated.
- Give workflows the minimum required token permissions.
- Separate pull-request validation from production deployment.
- Use GitHub environments for staging and production gates.

## Transfer checklist

1. Capture the source repository's collaborators, branches, open pull requests, issues, releases, webhooks, secrets, environments, deploy keys, and installed apps.
2. Back up local-only branches and uncommitted work.
3. Confirm external integrations that reference the current owner or repository URL.
4. Transfer the repository and verify redirects, remotes, actions, webhooks, Railway, Supabase, and monitoring.
5. Assign the responsible team and apply the repository ruleset.
6. Run a controlled validation before the first post-transfer release.
7. Record the new owner, deployment path, recovery procedure, and review date.
