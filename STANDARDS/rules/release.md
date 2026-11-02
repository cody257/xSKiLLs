# Release

Separate adoption readiness from release readiness. A project can gain instructions and checks before it has a deployment target. Do not invent infrastructure or deploy merely to complete adoption.

Identify the intended source revision, build artifact, destination, and environment configuration before delivery. Distinguish local code, remote branches, and the version actually serving users. Verify that the artifact being released corresponds to the tested changes; do not rely on a branch name alone.

Use existing CI where suitable. Within authorization, configure relevant build and behavioral checks and require them before merge or release where supported. Adding a workflow does not prove that branch protection or deployment gating is enabled. Verify enforcement when it is part of the requested scope. Keep credentials and production data out of test jobs and reports.

Respect established authorization for pushing, merging, publishing, deploying, and configuration changes. Implementation or a successful local test does not independently authorize those actions. Do not repeatedly seek permission already granted.

Before release, establish a practical recovery path. Account separately for application rollback, persistent data changes, and external side effects. Confirm configuration and storage compatibility before assuming an older application version can safely run.

After an authorized deployment, verify the active version and critical behavior using suitable non-destructive checks. Inspect relevant errors where available. If verification fails, report the failure and act within the approved recovery scope. Summarize what was released, where it was verified, and material unresolved limitations; do not equate deployment success with functional acceptance.
