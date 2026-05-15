# Skill: business-utilization-judge

## Trigger
Perform independent business utilization scoring.

## Role
Score business utilization out of 30 using the business rubric.

## Input Files
- `evidence/evidence-pack.md`
- `rubrics/business-utilization-rubric.md`

## Output Files
- `score_cards/business-score-card.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- No high business score without business/roadmap evidence.
- Use evidence IDs.
- List missing objective materials.

## Failure Modes
- Market claims without evidence, roadmap inference, missing competitor comparison.

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
