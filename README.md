# xSKiLLs

Seven project skills. Display names use the `x` prefix; invocation identifiers are lowercase.

| Display name | Invocation | Purpose |
| --- | --- | --- |
| xAdoption | `$xadoption` | Establish shared standards in new or existing projects |
| xBuild | `$xbuild` | Implement and verify an agreed outcome |
| xExperiment | `$xexperiment` | Resolve uncertainty through a bounded trial |
| xLearn | `$xlearn` | Understand behavior and compare options |
| xMaintain | `$xmaintain` | Inspect or fix existing project health |
| xRelease | `$xrelease` | Verify readiness and perform authorized delivery |
| xClose | `$xclose` | Confirm a session can safely end |

xClose can follow any skill when you are ready to end the session. It checks closure without repeating the preceding workflow or requiring a release.

## Installation

Copy the selected directories under `skills/` into your user-level skills directory or a project's `.agents/skills/`. Inspect existing installations before replacing anything. These names replace the earlier skill identifiers; preserve any local modifications when migrating.

For **xAdoption**, also retain the shared `STANDARDS/` directory. Its repository links work from this checkout. When installing elsewhere, rewrite the links in `skills/xadoption/SKILL.md` (and any skill that references shared files) to the permanent shared location. Keep one authoritative standards directory rather than copying it into every project.

The adoption template's `{{STANDARDS_ROOT}}` token is replaced with that verified location when creating a project's AGENTS.md. Project commands and exceptions remain local. The optional `csi-clean` skill is separate and is used only when available and a clean-copy workflow is needed.

Start a new turn or session after installation. Select a skill or mention its identifier. If discovery has not refreshed, restart the client. These files do not register literal slash commands.

## Shared standards

- `STANDARDS/rules/shared-behaviors.md` — common patterns used by every skill (clarifying questions, proportional scope, preserve work, finish reporting).
- `STANDARDS/rules/` — domain rules for testing, safety, quality, and release.
- `STANDARDS/templates/AGENTS.template.md` — starter for project AGENTS.md.

## Use and scope

These instructions preserve scope and existing authorization; they are not an access-control system. Adoption does not automatically authorize deployment or deletion of an old working copy.

Use [examples](examples/EXAMPLES.md), [trial examples](examples/TRIALS.md), and [feedback guidance](examples/FEEDBACK.md). See [CHANGELOG.md](CHANGELOG.md) and [VALIDATION.md](VALIDATION.md) for history.
