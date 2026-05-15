# Skill: invention-structurer

## Trigger
Convert extracted material into an invention map.

## Role
Map problem, solution, components, effects, implementation, and claim candidates.

## Input Files
- `extracted/document-summary.md`
- `extracted/image-observations.md`

## Output Files
- `invention/invention-map.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Separate inventor claims, evidence, and hypotheses.
- Do not create score claims.
- List missing implementation details.

## Failure Modes
- Problem-solution mismatch, unclear components, unsupported effects.

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
