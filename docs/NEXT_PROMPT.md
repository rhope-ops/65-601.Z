# Next prompt: 65-601.Z

Updated: 2026-11-25. Keep this file at 40 lines or fewer. The current request overrides it.

## State

- main: kit 11.1.0 (kit a629550, no v11.1.0 tag yet) since PR 15 (main 44e7815): role word "the Maintainer", `dod-security: on`.
- Branch `claude/kit-package-mode` (PR 16): package mode, 27 of 53 kit scripts from the `archimedes-kit` package. Lane C: the merge needs the Maintainer's approval. The fleet coordinator session gets the review result and takes the merge to the Maintainer.
- In package mode, run `scripts/check.sh --kit-install` after a new clone (the SessionStart hook does it at startup when the verify fails).

## Open (in order)

1. Merge PR 16, package mode (lane C).
2. Add the first project rules to AGENTS.md "Project rules".
3. The Maintainer names the instruction files: `audit-instructions:` lines in `.check`.
4. Kit follow-up: in package mode, `.github/workflows/security.yml` runs bandit with no `--kit-install` step, so it scans 26 of 53 kit scripts.

## Needs the Maintainer

- Approve the lane C merge of PR 16.
- Turn on private vulnerability reporting (on GitHub, the repo page **Settings**, section **Advanced Security**, **Private vulnerability reporting**: **Enable**), so SECURITY.md's first steps work.

## Do not

- Do not merge a lane C pull request without the Maintainer's approval.
