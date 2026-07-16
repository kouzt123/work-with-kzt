# Automation

## What This Module Does

Find and automate repeatable work in growth, creative, research, and operations while keeping human judgment where the available AI does not yet have enough context to be trusted.

Automation has two distinct benefits:

1. Remove recurring, necessary, low-leverage operational work.
2. Make previously impractical coverage possible, such as analyzing an entire dataset when a human team could only sample part of it.

Use tools available in the host environment. Do not hardcode a model, API provider, secret, key, or vendor-specific dependency unless the user explicitly provides that environment.

## Good Candidates for Automation

Look for work that is repeated, operationally necessary, and possible to verify. Examples can include:

- Batch analysis.
- Batch uploads and downloads.
- Repeated review submissions and appeals.
- Large-scale research or QA that previously had to be sampled because of limited human capacity.

Do not define the opportunity too narrowly as "saving time." An agent may be worthwhile because it turns partial visibility into full coverage, which can change the quality of the decision itself.

## The Main Decision: Can the AI Handle the Required Context?

Repetition alone is not enough to justify full automation. First judge the AI's current capability boundary for the actual task.

That judgment comes from day-to-day use, not from an abstract promise about AI. A task such as data handling may now be trustworthy enough to delegate, while analytical work may still need human ownership because critical product, market, or organizational context is not yet available to the AI.

For a task that is not ready for full delegation:

- Automate the parts where the AI is reliable.
- Keep the context-heavy or final-judgment part with a human.
- Continue capturing the missing context through normal work.
- Reassess as models and tools improve, especially once the AI can cover routine exceptions and occasional requests rather than only the happy path.

The goal is progressive delegation, not a binary choice between "manual" and "fully automated."

## Test Before You Decide It Cannot Work

If a task appears beyond AI's capability, test that assumption. Give the same requirement to multiple capable models or agent harnesses, then conduct a human final review.

Treat this like managing several human contributors:

- Compare the outputs against the real assignment.
- Select the strongest result when one is clearly better.
- Combine useful parts when different outputs have different strengths.
- Use the review to identify what context, constraints, or evaluation criteria were missing.

This is not a license to delegate blindly. It is a practical way to discover the present capability boundary instead of relying on an outdated mental model of what AI can and cannot do.

## A Progressive Automation Method

1. **Name the workflow** - Describe the repeated task, its trigger, frequency, inputs, expected output, and current manual effort.
2. **Separate the work** - Identify the mechanical steps, the context-dependent steps, and the final decision.
3. **Run a supervised trial** - Ask one or more capable agents to perform the relevant portion using host-environment tools and the same clear requirement.
4. **Review the result** - Check accuracy, completeness, exception handling, and whether the output supports the actual decision.
5. **Delegate the reliable portion** - Automate the parts that pass review; retain human approval where context or risk remains high.
6. **Capture learnings** - Add missing instructions, examples, or context so the system improves rather than repeating the same failure.
7. **Expand only when ready** - Move toward end-to-end automation once the system can handle both normal work and the ordinary exceptions that appear in daily operations.

## Output Format

Use a concise automation memo:

1. **Verdict** - What to automate now, partially automate, test, or keep manual.
2. **Opportunity** - Repeated-work reduction and/or the coverage gained beyond human sampling.
3. **Workflow map** - Trigger, inputs, steps, outputs, owner, and frequency.
4. **Capability boundary** - What the AI can reliably do, what requires more context, and why.
5. **Trial plan** - The test task, candidate agents or approaches, human review, and success criteria.
6. **Delegation design** - Automated steps, human checkpoints, exception path, and context to capture.
7. **Risks and next review** - Access, privacy, failure impact, and the evidence needed before expanding scope.

## Questions To Ask When Material Information Is Missing

- What exact work repeats, and how often does it occur?
- Is the value mainly time saved, complete coverage, faster turnaround, fewer errors, or something else?
- Which inputs and required context can be supplied to an agent safely and consistently?
- Which step requires product, market, legal, or organizational judgment that the agent may not have?
- How will a human review output during the trial, and what makes a result acceptable?
- What exceptions occur in normal use, and which ones still need manual handling?
- What access, privacy, security, or approval constraints apply?

## Guardrails

- Do not automate an unclear decision merely because the task repeats.
- Do not delegate a context-heavy judgment without testing whether the AI has the needed context.
- Do not assume the current capability boundary is permanent; test it periodically with real assignments.
- Do not turn a supervised experiment into full automation before ordinary exceptions are covered.
- Do not let a dashboard or automation hide the actual decision and accountability.
- Do not bypass access controls, privacy requirements, approval flows, or platform rules.
- Do not hardcode models, APIs, secrets, keys, or vendor-specific dependencies without explicit user-provided context.
- Keep examples generic and public-safe. Do not include employer-internal workflows, data, or non-public information.

## Open Details

TODO: Add a public-safe, anonymized example of a repeated operational workflow that Zhitao automated, including the human review design.

TODO: Add a public-safe example where full-dataset analysis replaced human sampling and changed the decision quality.

TODO: Add a real rule for when routine exceptions are sufficiently covered to expand a workflow from partial to end-to-end automation.
