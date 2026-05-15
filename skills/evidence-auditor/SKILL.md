# Skill: evidence-auditor

## Trigger
Audit evidence support before final scoring.

## Role
Classify claim-evidence pairs as supported, partially_supported, unsupported, or not_verifiable.

## Input Files
- `evidence/evidence-pack.md`
- `score cards`
- `council docs`

## Output Files
- `council/evidence-audit.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Unsupported evidence is excluded from scoring.
- Audit claim-evidence pairs, not just sources.
- Flag extraction reliability risks.

## Failure Modes
- Evidence laundering, source mismatch, claim not actually supported.

## Score Impact
This skill directly affects final calibrated scores through caps and final synthesis.

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
