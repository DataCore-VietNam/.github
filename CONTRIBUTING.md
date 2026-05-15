# Contributing to DataCore VietNam

Thanks for taking the time to contribute. This guide applies to every
repository in the DataCore-VietNam organization unless a repository provides
its own `CONTRIBUTING.md`.

## Getting started

1. Fork the repository and create a branch from `main`.
2. Use a descriptive branch name: `feature/...`, `fix/...`, or `docs/...`.
3. Install dependencies and run the test suite before making changes.

## Development workflow

- Keep changes focused — one logical change per pull request.
- Write or update tests for any behavior change.
- Run linters and formatters locally before pushing.
- Ensure CI passes; the org-wide workflow templates run lint, build, and tests.

## Commit messages

Write clear, imperative commit messages:

```
Add reconciliation step to price pipeline

Explain the why, not just the what, when it is not obvious.
```

## Pull requests

- Fill out the pull request template completely.
- Link any related issues with `Closes #123`.
- A maintainer review and green CI are required before merge.
- Squash-merge is the default unless a maintainer says otherwise.

## Reporting bugs and requesting features

Open an issue using the provided templates. Include reproduction steps,
expected vs. actual behavior, and environment details.

## Code of conduct

All contributors must follow the [Code of Conduct](CODE_OF_CONDUCT.md).
