# Skill: patentability-judge

## Trigger
Assess patentability and claim risk.

## Role
Review novelty, inventive step, claim breadth, and prior-art risk as risk assessment only.

## Input Files
- `invention/invention-map.md`
- `attorney review`
- `evidence/evidence-pack.md`

## Output Files
- `score_cards/patentability-review.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Do not provide legal advice.
- Use risk levels.
- Identify score cap implications.

## Failure Modes
- Insufficient prior art, no claim draft, attorney review unavailable.

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
