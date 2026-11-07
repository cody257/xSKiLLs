---
name: xadoption
description: Establish shared engineering standards in a new or existing project, including missing agent instructions, applicable checks, and optional clean-copy reconciliation. Use when adopting a project into this foundation.
---

# xAdoption

Adopt the selected project incrementally. Preserve working behavior and unique work; adoption does not require a restart, rewrite, or deployment.

Follow [shared behaviors](../../STANDARDS/rules/shared-behaviors.md). Read applicable shared references before acting:

- [Testing](../../STANDARDS/rules/testing.md): behavioral coverage and test evidence.
- [Safety](../../STANDARDS/rules/safety.md): data, access, secrets, and recovery.
- [Quality](../../STANDARDS/rules/quality.md): acceptance, builds, usability, and review.
- [Release](../../STANDARDS/rules/release.md): CI and authorized delivery.

Inspect applicable instructions, the checkout, existing checks, and relevant local, remote, and deployed versions. Establish the requested adoption scope and observable completion criteria. If the user supplied a goal, use those criteria to assess completion; do not substitute file creation for a working foundation.

Use the current folder unless a clean copy is requested or justified. When needed, use the available `csi-clean` skill. Preserve the original and reconcile unique work before considering retirement. Do not delete the original through this workflow.

If project-root AGENTS.md is missing, create it from the [default template](../../STANDARDS/templates/AGENTS.template.md). Otherwise preserve project-specific guidance and reconcile missing references without duplication. Respect inherited instructions. Replace the template's standards-root token with the verified shared directory. Keep unknown project facts explicitly unresolved.

Links resolve from this skill directory. When installing elsewhere, update these references and project links to the shared directory; maintain one authoritative copy. Flag inaccessible references rather than inventing their contents.

Establish proportionate checks within scope. Empty projects need a foundation, not invented commands or infrastructure. Finish with changes, verification evidence, and unresolved gaps. Reuse valid checks; retain existing authorization boundaries.

**Hand-off:** After a solid foundation exists, suggest xBuild for new capabilities, xMaintain for health issues, or xLearn for deeper understanding. Do not expand into implementation unless requested.
