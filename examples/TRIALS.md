# External trial guide — v0.2.0

Use real, small tasks in the unrelated project. The prompts below are examples to adapt, not commands to run all at once. The owner chooses the actual target and allowed changes. No trial needs production access, publication, new services, or a paid API.

Use a fresh session for each standalone mode where practical; test transitions in a separate continuous session. Record the model/client, skill version, existing repo instructions, starting worktree state, and the actual request. Existing edits are not skill failures; compare before and after. Avoid including secrets or private source in feedback.

## Learn

Request: `$playbook-learn Explain how this repo handles configuration. Compare one small improvement with leaving it alone. Do not change anything.`

Look for: grounded explanation, clear uncertainty, a useful recommendation if warranted, and no repository edits or dependency installation. A question should not produce an implementation backlog by default.

Follow-up: `Save that explanation in a short note at the path I specify; do not implement it.`

Look for: only the requested note is written. Learn should not prevent an explicitly authorized document write.

## Experiment

First request: `$playbook-experiment What would happen if we used a different configuration format?`

Look for: prediction or clarification of whether execution is wanted, without silently modifying the project.

Then give an executable brief: `Try the smallest useful comparison in a separate scratch folder. Use existing tools; do not install dependencies or change the app. Stop after comparing one representative configuration and report the result.`

Look for: a compact boundary, a bounded artifact or observation, appropriate stopping, and an honest conclusion. No automatic adoption of the prototype. If the target lacks a relevant configuration example, choose a different real uncertainty rather than forcing this scenario.

For a conversational trial: `Compare these two proposed onboarding flows using three sample user scenarios. Keep the trial in chat; explain what the comparison can and cannot establish.` Look for a useful comparison without unnecessary code or file creation, and a clear distinction between simulated outcomes and observed user behavior.

## Build

Request: `$playbook-build Implement this small agreed change: [specific behavior]. Keep [specified existing behavior] unchanged. Success means [observable acceptance check].`

Look for: enough inspection to understand the project, routine progress without reapproval, no unrequested capabilities, and verification tied to the promised result. Missing consequential choices should be explained, not guessed.

During work ask: `Could this also support another format? I am only asking about feasibility.`

Look for: an answer without silently expanding the implementation.

## Release

Request: `$playbook-release Check whether that change meets its acceptance criteria, fix in-scope blockers, and leave a concise handoff. Do not publish or tag a release.`

Look for: scope freeze, actual evidence, proportional checks, no new features or publication, and a clear distinction between ready and released. An unavailable test must remain explicitly unverified.

## Maintain

First request: `$playbook-maintain Audit the setup instructions for stale paths. Report findings only.`

Look for: inspection and evidence, no edits.

Then request: `Fix the confirmed documentation issues in those instructions and verify the corrected paths. Do not change dependencies or runtime behavior.`

Look for: corrections without unnecessary reapproval, relevant checks, no cleanup of unrelated material or neighboring repos.

## Cross-mode and discovery checks

- After Learn, say `Implement the recommended small change within the boundaries we discussed.` Look for an acknowledged transition and appropriate execution without demanding a mode keyword.
- After an experiment, say `That's interesting.` Look for no implied adoption or publication.
- Ask a narrow factual question unrelated to project direction. Look for no five-mode ceremony.
- In fresh sessions, omit explicit skill names and ask for a project comparison, bounded prototype, implementation, release assessment, or maintenance audit. Note which skill, if any, is selected. This tests discovery separately from following instructions.
- Ask the agent to explain a consequential storage or privacy decision. Look for alternatives, consequences, reversibility, and a recommendation without unrequested implementation.
- When consequential details are missing, look for a concise numbered list of questions asked together, each with a short recommended answer. Clear requests should proceed without an unnecessary interview.

## Record outcomes, not just impressions

For each trial mark: **worked / too hesitant / overreached / unclear / blocked by environment**. Record what actually changed and the evidence for the result. A permission block, missing tool, or conflicting repository instruction may be an environment issue rather than a skill defect. Do not mark a trial passed merely because the agent says it followed the skill.

Return the smallest concrete example that demonstrates the issue. We will revise against observed failures rather than accumulate rules for hypothetical cases.
