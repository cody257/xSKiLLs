# Safety

Preserve unique work before changing project structure. Inspect uncommitted changes, untracked files, local commits, and relevant ignored configuration. Do not assume a remote repository or apparently newer folder contains everything valuable. Keep a recoverable original when reconciling copies.

Use isolated test data for operations that write, delete, import, synchronize, or migrate records. A branch does not isolate databases, accounts, email recipients, or external services. Verify the actual target before running commands that mutate state.

For affected data workflows, check repeated execution, interrupted writes, conflicts, and preservation of later user decisions. Prefer atomic replacement or transactions where appropriate. Establish a usable backup and recovery method before consequential changes; verify restoration when the risk warrants it. Reverting code alone may not restore data.

Keep credentials, tokens, private identifiers, and personal data out of commits, logs, screenshots, traces, and shared artifacts. Restore configuration through appropriate secret storage rather than copying sensitive values into instructions.

Enforce access permissions at service boundaries, including resource ownership. Validate inputs and apply suitable size, processing-time, and resource limits. Assess relevant dependency advisories by actual exposure; avoid blind upgrades and unrelated dependency churn.

Respect the user's authorized scope. Preparation and local verification do not independently authorize publishing, messaging, production changes, or destructive actions. Existing authorization remains valid; do not request it repeatedly. Surface concrete unresolved risks without expanding routine work into an unsolicited security audit.
