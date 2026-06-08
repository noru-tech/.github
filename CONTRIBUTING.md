# Contributing to Noru

Thanks for your interest in contributing! Noru builds a continuous, agentic compliance
platform, and our open repositories include integrations, tooling, and examples that the
community can improve. These guidelines apply across all repositories in the `noru-tech`
organization.

## Code of Conduct

This project and everyone participating in it is governed by our
[Code of Conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold it.

## Ways to Contribute

- **Report bugs** — Open an issue using the bug report template.
- **Request features** — Open an issue using the feature request template.
- **Improve docs** — Documentation fixes are always welcome and a great first contribution.
- **Submit code** — Fix a bug or implement an agreed-upon feature via a pull request.

> Found a security issue? **Do not** open a public issue. Follow our
> [Security Policy](SECURITY.md) instead.

## Before You Start

For anything beyond a small fix, please open an issue first so we can discuss the approach.
This avoids duplicated effort and helps us keep contributions aligned with the roadmap —
which matters especially for compliance-related logic, where correctness and traceability
are non-negotiable.

## Development Workflow

1. **Fork** the repository and create your branch from `main`.
2. Use a descriptive branch name, e.g. `fix/control-mapping-typo` or
   `feat/azure-evidence-sync`.
3. Make your changes in small, logically grouped commits.
4. Follow the existing code style and conventions in the repository.
5. Add or update tests for any behavior you change.
6. Update documentation when you change user-facing behavior.
7. Ensure the test suite and linters pass locally.

## Commit Messages

We follow [Conventional Commits](https://www.conventionalcommits.org/):

```
feat: add NIS2 control mapping
fix: correct evidence timestamp on GCP sync
docs: clarify MCP setup steps
```

## Pull Requests

- Keep PRs focused; one logical change per PR.
- Fill out the pull request template completely.
- Link the issue your PR addresses (e.g. `Closes #123`).
- Ensure CI is green before requesting review.
- Be responsive to review feedback — we aim to review promptly in return.

By submitting a contribution, you agree that it may be licensed under the same license as
the repository you are contributing to.

## Questions?

See [SUPPORT.md](SUPPORT.md) for the best way to get help.
