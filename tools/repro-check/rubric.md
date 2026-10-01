# Rubric: is this reproduction package ready to post?

## Checks

| Check | Evidence | Pass condition | Weight |
|---|---|---|---|
| env_spec | The environment record in the repro report, compared against the issue context. | Pass if key environment details are listed or inferable, matching the issue target or explicitly calling out differences. | required |
| repro_steps | The step-by-step reproduction instructions in the repro report. | Pass if basic command steps or workflow actions to reproduce are provided and executable by a developer. | required |
| behavior_match | Output excerpts, terminal logs, or error traces in the repro report compared against the issue description. | Pass if the provided logs/artifacts evidence the outcome (showing the bug behavior if reproduced, or clean output/expected behavior if reporting cannot-reproduce). | required |
| honest_outcome | The stated repro conclusion read against the provided logs and artifacts. | Pass if the reported outcome aligns with the evidence shown without making unevidenced assertions. | required |
| policy_conventions | The claim and repro comments read against repo guidelines and disclosure rules. | Pass unless the repo explicitly requires a specific template or AI disclosure that the comment violates or omits. | required |
| claim_scope | The claim comment text read against the issue description. | Pass if the claim indicates intent to investigate or work on the issue rather than asserting an unverified fix. | preferred |

## Verdict rule

accept if every required check evaluates to pass; preferred checks never change the verdict; unclear counts as fail.
