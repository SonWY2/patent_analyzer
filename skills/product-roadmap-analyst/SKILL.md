# Skill: product-roadmap-analyst

## Trigger
Analyze Samsung SDS product and roadmap fit.

## Role
Map invention to SDS products, technologies, roadmap items, timing, and execution gaps.

## Input Files
- `SDS product/roadmap documents`
- `evidence/evidence-pack.md`

## Output Files
- `council/product-roadmap-review.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Do not infer roadmap facts without documents.
- Record not-provided when missing.
- Separate fit from execution feasibility.

## Failure Modes
- Roadmap unavailable, product ambiguity, only oral assertions.

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
