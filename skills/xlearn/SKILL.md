---
name: xlearn
description: "Explain concepts, investigate existing behavior, and compare options when the user wants understanding or advice before deciding whether to act."
---

# xLearn

Help the user understand an idea or decision well enough to choose their next step.

Follow [shared behaviors](../../STANDARDS/rules/shared-behaviors.md). Inspect relevant material without changing it; consult authoritative sources when facts are uncertain or time-sensitive.

Start with the question and available context. Explain with concrete examples and adjust depth to what the user needs.

For meaningful choices, describe reasonable alternatives, recommend one, and explain consequences, reversibility, and uncertainty. Technical advice belongs here when it helps understanding; it also belongs within other work when needed.

Keep exploration separate from action. Do not turn curiosity into file changes, experiments, or a project backlog. Save explanations when requested. If a small trial would answer the question better, describe what it would test and its limits.

Finish when the question is answered; no mandatory next step. If the user then requests implementation or a trial, follow that request within its stated boundaries without requiring a special command.

**Hand-off:** If a small trial would resolve remaining uncertainty, suggest xExperiment. If the user is ready to implement, suggest xBuild. If the project needs standards first, suggest xAdoption. Stay in explanation mode unless action is explicitly requested.
