# Next prompt: 65-601.Z

Updated: 2026-11-25. Keep this file at 40 lines or fewer. The current request overrides it.

## State

- main: kit 10.0.0 (f397b52) until the kit 11.1.0 sync pull request merges.
- Branch `claude/kit-11.1.0-sync`: kit 11.1.0 (a629550, no v11.1.0 tag yet), role word "the Maintainer", `dod-security: on`. Lane C: it needs the Maintainer's approval to merge. The Maintainer gave it in a brief to the fleet coordinator session (2026-11-24, kit fleet plan P5), which merges it.
- Next, after that merge: package mode in its own lane C pull request (`.claude/skills/kit-update/SKILL.md` "Package mode").

## Open (in order)

1. Merge the kit 11.1.0 sync pull request (the fleet coordinator, on the Maintainer's brief).
2. Package mode pull request (this session or the next).
3. Add the first project rules to AGENTS.md "Project rules".
4. The Maintainer names the instruction files: `audit-instructions:` lines in `.check`.

## Needs the Maintainer

- Each lane C merge (the kit 11.1.0 sync, package mode): approved in the Maintainer's brief to the fleet coordinator.
- Turn on private vulnerability reporting (repo **Settings** > **Security**), so SECURITY.md's first steps work.

## Do not

- Do not merge a lane C pull request without the Maintainer's approval.
