# Skill: technical-excellence-judge

## Trigger
Perform independent technical scoring.

## Role
Score technical excellence out of 30 using the technical rubric.

## Input Files
- `invention/invention-map.md`
- `evidence/evidence-pack.md`
- `rubrics/technical-excellence-rubric.md`

## Output Files
- `score_cards/technical-score-card.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Use evidence IDs for every score-bearing rationale.
- Do not use unsupported creative hypotheses.
- List cap risks.

## Failure Modes
- Evidence IDs missing, novelty conflated with business value, unsupported high score.

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
