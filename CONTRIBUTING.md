# Contributing

## Commits

Conventional Commits: `type: description` — lowercase, no trailing period, no scope. Types: `feat`, `fix`, `docs`, `chore`, `refactor`, `test`. Default branch is `main`; PRs squash-merge, so the PR title becomes the commit message and must pass the same format.

## Attribution

Every commit names its authors. The primary author goes in the git author field; every other contributor — agent or human — gets a `Co-Authored-By` trailer. Agents identify themselves with their model id:

```
feat: resolve provider targets from module manifest

Co-Authored-By: Claude Fable 5 (claude-fable-5) <claude@martinzeman.net>
Co-Authored-By: Codex (gpt-5.5) <codex@martinzeman.net>
```

An agent working alone commits under its own author identity, no trailer needed. History must answer "who wrote this" without archaeology.

## Review

Nothing merges on a single opinion:

1. Automated review bots comment on every PR.
2. Cross-vendor agent review — at least one agent from a different vendor than the author reads the diff.
3. A human approves and merges.

## Checks

Run `make validate` before pushing; CI runs the same checks. Hooks activate with `make install` after cloning. Never bypass a failing hook — fix the cause or fix the check.
