# Skill: devil-advocate

## Trigger
Challenge high scores and maximum-score candidates.

## Role
Find weaknesses, overclaims, alternative explanations, unresolved risks, and missing evidence.

## Input Files
- `all score cards`
- `evidence/evidence-pack.md`
- `creative/creative-hypotheses.md`

## Output Files
- `council/devil-advocate.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Always challenge max-score candidates.
- Assign severity.
- Do not make vague objections.

## Failure Modes
- Formalistic challenge, no severity, no resolution path.

## Score Impact
This skill provides inputs or provisional judgments that Score Chair may use after evidence audit.

## Handoff
End with:

```md
## Handoff
- Key Findings:
- Evidence IDs Used:
- Missing Information:
- Cap or Gate Concerns:
- Recommended Next Skill:
```
