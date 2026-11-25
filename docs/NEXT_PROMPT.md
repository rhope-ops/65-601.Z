# Next prompt: 65-601.Z

Updated: 2026-11-25. Keep this file at 40 lines or fewer. The current request overrides it.

## State

- main: kit 10.0.0 (f397b52) until the kit 11.1.0 sync pull request merges.
- Branch `claude/kit-11.1.0-sync`: kit 11.1.0 (a629550, no v11.1.0 tag yet), role word "the Maintainer", `dod-security: on`. Lane C: the merge needs the Maintainer's approval. The fleet coordinator session gets the review result and takes the merge to the Maintainer.
- Next, after that merge: package mode in its own lane C pull request (`.claude/skills/kit-update/SKILL.md` "Package mode").

## Open (in order)

1. Merge the kit 11.1.0 sync pull request (lane C: the Maintainer approves; the fleet coordinator handles it).
2. Package mode pull request (this session or the next).
3. Add the first project rules to AGENTS.md "Project rules".
4. The Maintainer names the instruction files: `audit-instructions:` lines in `.check`.

## Needs the Maintainer

- Approve each lane C merge (the kit 11.1.0 sync, then package mode).
- Turn on private vulnerability reporting (on GitHub, the repo page **Settings**, section **Advanced Security**, **Private vulnerability reporting**: **Enable**), so SECURITY.md's first steps work.

## Do not

- Do not merge a lane C pull request without the Maintainer's approval.
