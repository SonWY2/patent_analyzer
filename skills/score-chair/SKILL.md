# Skill: score-chair

## Trigger
Calibrate final scores.

## Role
Apply evidence audit, score caps, and max-score gates to determine final scores.

## Input Files
- `all reviews`
- `council/evidence-audit.md`
- `rubrics/max-score-gate.md`
- `rubrics/score-cap-rules.md`

## Output Files
- `council/score-calibration.md`
- `council/chair-synthesis.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Do not average scores mechanically.
- Use lowest applicable cap unless justified.
- Maximum score requires gate pass.

## Failure Modes
- Cap omitted, unsupported evidence counted, Devil Advocate ignored.

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
