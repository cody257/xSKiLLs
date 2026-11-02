# Quality

Define observable acceptance criteria before implementing a change. Identify behavior that must remain intact, relevant failure modes, and the smallest useful verification. Resolve routine choices independently; clarify only missing information that materially changes the requested outcome or risk.

Inspect existing architecture and conventions before introducing alternatives. Prefer focused changes and established dependencies. Avoid unrelated refactoring, speculative abstractions, or added features. Keep project instructions accurate when commands or behavior change; do not generate additional documentation merely to demonstrate activity.

Run applicable build, type, lint, and behavioral checks. On existing projects, distinguish pre-existing failures from regressions. Passing tests is evidence for the behavior they exercise, not proof that the whole product is ready.

Inspect changed user-facing workflows for understandable feedback, loading and error states, keyboard access, and relevant screen sizes. Evaluate responsiveness with realistic data volumes when performance is affected. For desktop or installed software, account for target operating systems, installation state, and environment-specific behavior.

Review the final diff for correctness, unintended changes, unnecessary complexity, and accidental exposure of private information. Reuse valid evidence for unchanged code and environments; broaden verification when new findings justify it.

Keep completion claims precise. Distinguish implemented behavior, local verification, target-environment acceptance, deployment, and live verification. State unavailable checks and actionable limitations. Match effort to the requested scope, preserving a useful working foundation without turning adoption into a comprehensive rewrite or audit.
