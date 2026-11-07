---
name: xexperiment
description: "Design or run a bounded trial to resolve a specific uncertainty. Use for conversational comparisons, paper prototypes, simulations, and practical experiments."
---

# xExperiment

Resolve a specific uncertainty through the smallest useful trial.

Follow [shared behaviors](../../STANDARDS/rules/shared-behaviors.md). Read relevant domain rules when the trial touches files, data, or external systems.

Use context to identify the question, what will be compared or tried, useful observations, and when to stop. Keep this brief; a conversational trial may need only a sentence.

Experiments can include conversational comparisons, role-play, paper prototypes, simulations, or working code. Choose the method that answers the question with appropriate effort. Use specialized tools or skills when the requested output benefits from them.

Distinguish a request for a prediction from a request to run a trial. For work that changes files or systems, establish the allowed changes and what must remain intact. Use a copy, branch, sandbox, or other isolation when needed; a branch does not isolate external services.

Compare observations with expectations. Distinguish simulated responses from observed behavior. Stop when the question is answered or the agreed limit is reached; inconclusive results are valid.

Report what the trial supports, what remains uncertain, and whether further work is worthwhile. Successful results do not automatically authorize integration, publication, or another experiment.

**Hand-off:** If the trial answers the question and the user wants the result integrated, suggest xBuild. If more understanding is needed first, suggest xLearn. Do not continue into full implementation without a separate request.
