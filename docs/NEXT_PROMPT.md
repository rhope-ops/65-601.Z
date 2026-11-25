# Next prompt: 65-601.Z

Updated: 2026-11-25. Keep this file at 40 lines or fewer. The current request overrides it.

## State

- main: kit 10.0.0 (f397b52) until the kit 11.1.0 sync pull request merges.
<<<<<<< HEAD
- Branch `claude/kit-11.1.0-sync`: kit 11.1.0 (a629550, no v11.1.0 tag yet), role word "the Maintainer", `dod-security: on`. Lane C: it needs the Maintainer's approval to merge. The Maintainer gave it in a brief to the fleet coordinator session (2026-11-24, kit fleet plan P5), which merges it.
- Branch `claude/kit-package-mode` (on top of the sync branch): package mode, 27 of 53 kit scripts from the package. Lane C. Merge it after the sync pull request. After a clone or branch switch, run `scripts/check.sh --kit-install` (the SessionStart hook does it when the verify fails).

## Open (in order)

1. Merge the kit 11.1.0 sync pull request (the fleet coordinator, on the Maintainer's brief).
2. Merge the package mode pull request (the fleet coordinator, on the Maintainer's brief), after item 1.
=======
- Branch `claude/kit-11.1.0-sync`: kit 11.1.0 (a629550, no v11.1.0 tag yet), role word "the Maintainer", `dod-security: on`. Lane C: the merge needs the Maintainer's approval. The fleet coordinator session gets the review result and takes the merge to the Maintainer.
- Next, after that merge: package mode in its own lane C pull request (`.claude/skills/kit-update/SKILL.md` "Package mode").

## Open (in order)

1. Merge the kit 11.1.0 sync pull request (lane C: the Maintainer approves; the fleet coordinator handles it).
2. Package mode pull request (this session or the next).
>>>>>>> claude/kit-11.1.0-sync
3. Add the first project rules to AGENTS.md "Project rules".
4. The Maintainer names the instruction files: `audit-instructions:` lines in `.check`.

## Needs the Maintainer

<<<<<<< HEAD
- Each lane C merge (the kit 11.1.0 sync, then package mode): approved in the Maintainer's brief to the fleet coordinator.
- Turn on private vulnerability reporting (repo **Settings** > **Security**), so SECURITY.md's first steps work.
=======
- Approve each lane C merge (the kit 11.1.0 sync, then package mode).
- Turn on private vulnerability reporting (on GitHub, the repo page **Settings**, section **Advanced Security**, **Private vulnerability reporting**: **Enable**), so SECURITY.md's first steps work.
>>>>>>> claude/kit-11.1.0-sync

## Do not

- Do not merge a lane C pull request without the Maintainer's approval.
