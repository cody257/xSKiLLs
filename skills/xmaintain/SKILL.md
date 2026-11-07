---
name: xmaintain
description: "Inspect or improve an existing project's health through bounded bug fixes, documentation corrections, and justified upkeep while preserving intended behavior."
---

# xMaintain

Keep an existing project reliable and understandable without turning upkeep into a new development cycle.

Follow [shared behaviors](../../STANDARDS/rules/shared-behaviors.md). Read relevant domain rules (especially testing, safety, and quality) when applying fixes.

Establish whether the user wants findings, specific fixes, or broader maintenance within stated boundaries. An inspection request calls for findings; a repair request authorizes the routine work needed to fix the issue.

Inspect relevant behavior, project records, and existing changes. Confirm defects and documentation drift before proposing corrections. Separate actual problems from optional improvements, new capabilities, and speculative concerns.

Choose the smallest adequate correction, using existing tools and conventions where practical. Explain consequential changes to compatibility, storage, access, or dependencies before proceeding beyond the established scope.

Carry out authorized fixes and verify the behavior they affect. Preserve unrelated work and historical releases. Do not upgrade everything merely because newer versions exist or delete meaningful material under the label of cleanup.

Update existing documentation when the change makes it inaccurate. Keep maintenance records proportional to the work; avoid duplicate handoffs.

Report what changed, what was checked, and any remaining issue with its practical impact. Present worthwhile larger improvements as options. Finish when the requested maintenance outcome is satisfied.

**Hand-off:** If a fix requires new capability work, suggest xBuild. If the project lacks shared standards, suggest xAdoption. If the result needs release verification, suggest xRelease. Do not expand into feature development.
