# Playbook skills — v0.2.0

Five portable skills for directing AI-assisted projects: Learn, Experiment, Build, Release, and Maintain. They help an agent understand intent, explain consequential choices, complete authorized work, and preserve useful context.

**Status:** v0.2.0, available for use. Structural validation and installation checks passed in Codex. These are instructions, not an access-control system or a guarantee of agent behavior.

## The five skills

| Skill | Use it to… | Example request |
| --- | --- | --- |
| `playbook-learn` | Understand and compare before changing things | `$playbook-learn Explain how this project works and where its risks are. Investigation only.` |
| `playbook-experiment` | Resolve uncertainty through a bounded trial | `$playbook-experiment Try a small prototype in a scratch directory. Keep the application unchanged; report the result and limitations.` |
| `playbook-build` | Deliver a requested capability | `$playbook-build Implement the agreed change and verify its acceptance criteria.` |
| `playbook-release` | Finish an implemented scope with evidence | `$playbook-release Check readiness and fix in-scope blockers. Prepare a handoff; do not publish.` |
| `playbook-maintain` | Keep existing work accurate and healthy | `$playbook-maintain Fix the stale setup instructions and check the corrected steps.` |

“Experiment — what would happen if…” may still be a conceptual question. The selected mode does not replace a clear target or permission boundary. Conversely, “implement that approach” can authorize a transition without a special command.

All skills can be selected explicitly. Normal automatic discovery is left enabled; descriptions distinguish their intended use. For the first experiment, select each one explicitly so you know which behavior you are evaluating. Then try ordinary-language requests to evaluate discovery separately.

## Try them in another repository

Each directory under `skills/` is a complete, independently usable skill. It contains `SKILL.md` plus `agents/openai.yaml` UI metadata. There are no runtime scripts, dependencies, API keys, hosted services, or references back to this checkout.

If the skills are already installed at user scope, use them across projects without copying them into each repository. Otherwise, download or clone [cody257/Playbook](https://github.com/cody257/Playbook) and follow the steps below for a project-scoped installation.

1. Copy the five `skills/playbook-*` directories into the target repository's `.agents/skills/` directory. Preserve each folder name and its contents. Check for existing folders first; do not overwrite another installation blindly. This changes only the target's skill configuration, not its application code. Check your target repo's policy before committing these files.
2. Start a fresh session in that repository. Use the skill picker or mention the skill by its supported name. Codex CLI/IDE support `$playbook-learn` and `/skills`; other clients may use a different picker. These files do **not** register literal `/learn` or `/experiment` commands.
3. Confirm the intended skill is available. If discovery has not refreshed, restart the client. For a direct-file trial, ask the agent to read and follow the selected `SKILL.md`; that tests its instructions, but not automatic skill discovery.
4. Use [the trial guide](examples/TRIALS.md). Keep the test bounded to a suitable unrelated repository or disposable copy; this package grants no authority to mutate that repository by itself.
5. Bring back [a feedback record](examples/FEEDBACK.md), especially examples of unnecessary hesitation, scope expansion, or missed transitions.

A useful setup request to the agent in the target project:

> Install the five Playbook skill folders from the package I provide into this repo's .agents/skills directory. Inspect existing skills first and do not overwrite collisions. Preserve application files. Confirm the available skill names, then wait for my first trial request.

To remove the experiment, remove only the five directories you installed after checking for local changes you want to keep. Project changes made while testing the skills are separate and need their own review; uninstalling a skill does not undo them.

For a user-scope installation, ask your agent to install all five folders under `skills/` from this repository using its skill installer. Check for existing versions before replacing them. Installation on one device does not configure another device.

Official setup and invocation reference, checked October 31, 2026: [Build skills](https://learn.chatgpt.com/docs/build-skills).

## What this version deliberately preserves

- Learning remains read-only by default; an explicitly requested saved explanation is allowed.
- Experiment, Build, Release, and Maintain can guide writes when the actual task authorizes them.
- Consequential decisions get explanations; routine authorized work does not need repeated approval.
- Each skill respects prior authorization and the requested scope.
- Maintenance distinguishes inspection from fixing. Release distinguishes readiness from publication.
- Existing project documents are reused; no mandatory STATE.md, DECISIONS.md, or handoff file is imposed.

Each skill is self-contained and remains between 150 and 250 words, including metadata. When clarification is needed, it asks concise numbered questions together, each with a short recommended answer. No sibling skill or mandatory interview is required.

## Scope

This repository contains the five skills and their usage and testing documentation. Website code and MCP integrations are separate work. Success is evidence of better behavior in realistic tasks, not merely valid Markdown.

The skills were developed by Cody from the AI Project Playbook, Shared AI Coding-Agent Operating Standard, and subsequent design discussions. The website and original working documents are not included.

No license file has been selected for this version.

See [VALIDATION.md](VALIDATION.md) for exactly what has and has not been checked.
