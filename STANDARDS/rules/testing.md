# Testing

Prefer real UI/API end-to-end tests for critical journeys. Exercise owned services rather than mocking them. Stub true third parties when appropriate, and state which integration behavior remains unverified. Test data changes in isolated environments with disposable records.

Use focused integration or unit tests where they verify behavior more efficiently, especially logic with many edge cases. Identify relevant failure cases first and prefer test-first development. Useful coverage may also be added after implementation.

Scale coverage to the change's risk. Significant workflows need a realistic multi-step scenario and relevant empty, boundary, invalid, unauthorized, and failure paths. Do not manufacture unrelated scenarios merely to satisfy a checklist.

Assert meaningful expected outcomes derived from requirements. Justify tolerances and ranges. Never branch on observed results to bypass assertions. Avoid tautological tests, mock-setup restatements, and checks tied to harmless implementation changes. Add regression tests for genuine coverage gaps; improve existing coverage when it already addresses the behavior.

Keep tests independent, repeatable, and controlled, including data setup and cleanup. Use bounded waiting for asynchronous behavior rather than arbitrary delays. Demonstrate that new tests detect their intended failures; preimplementation red counts. Use deliberate breakage selectively in isolated local copies, and restore behavior afterward.

Diagnose failures. Distinguish product defects, incorrect tests, environment problems, and pre-existing failures. Do not conceal failures through skips, weakened assertions, or retries until green. Diagnostic reruns are allowed; report instability that remains.

Provide exact rerun commands and relevant reports or traces, excluding secrets and private data. Identify the tested version and environment when results could otherwise be confused. Reuse valid evidence for unchanged behavior; rerun checks when changes or unresolved concerns justify it.
