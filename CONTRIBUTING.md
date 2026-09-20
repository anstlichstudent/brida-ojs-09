# Contributing

## Branches

- `main` contains deployable releases only.
- `develop` is the integration branch.
- Develop work on short-lived `feature/<name>` or `fix/<name>` branches, merge them into `develop`, then delete them.
- Promote `develop` to `main` only after every required check passes.

## Commits

Use atomic commits written in English:

```text
<type>(<optional-scope>): <imperative summary>
```

Allowed types:

- `feat`: add user-facing behavior
- `fix`: correct broken behavior
- `refactor`: change structure without changing behavior
- `test`: add or update tests
- `docs`: update documentation
- `chore`: maintain tooling or the project

Examples:

```text
feat(auth): add applicant login
fix(submission): prevent duplicate submission
chore: update dependencies
```

## Checks

Before each commit:

1. Run `php artisan test --compact`.
2. When PHP files changed, run `vendor/bin/pint --dirty --format agent`.
3. When frontend assets changed, run `npm run build`.

Commit only when every relevant check passes.

## Releases

- Merge `develop` into `main` with a release merge commit such as `chore(release): prepare release`.
- Tag each deployed release using Semantic Versioning, for example `v0.2.0` or `v0.2.1`.
