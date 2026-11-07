# Skill examples

Short illustrations of when and how each skill is typically used. These are not required project records.

## xAdoption

**Request:** "Adopt this repo into our standards and create an AGENTS.md if it's missing."

**Expected:** Inspects the checkout, creates or reconciles AGENTS.md from the template, links the shared standards, establishes proportionate checks, and reports gaps. Does not rewrite the project or authorize deployment.

## xBuild

**Request:** "Add a CSV export for the reports page and verify it works with the existing data."

**Expected:** Recovers constraints, implements the export in increments, verifies the behavior, updates records if needed, and stops. Asks clarifying questions only when the outcome would change.

## xExperiment

**Request:** "Which of these two caching approaches is simpler for our read-heavy endpoint? Try both briefly."

**Expected:** Designs the smallest useful comparison, isolates if needed, reports what the trial supports and what remains uncertain. Does not integrate the winner without a separate request.

## xLearn

**Request:** "Explain how the current auth middleware decides which routes are public, and what the tradeoffs are if we switch to a different library."

**Expected:** Inspects the relevant code without changing it, explains with concrete examples, compares options with consequences, and finishes. Does not implement the change.

## xMaintain

**Request:** "The nightly backup job is failing with a permissions error. Inspect and fix it."

**Expected:** Confirms the defect, applies the smallest adequate fix, verifies the affected behavior, updates inaccurate docs if any, and reports what changed. Avoids unrelated upgrades.

## xRelease

**Request:** "We're ready to ship the export feature. Check acceptance and prepare the handoff."

**Expected:** Holds scope steady, verifies the behavior users will rely on, clears routine blockers, records evidence and limitations, and prepares or performs the authorized delivery. Does not reopen feature work.
