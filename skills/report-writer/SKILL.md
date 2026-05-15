# Skill: report-writer

## Trigger
Generate committee-ready final report.

## Role
Assemble final report without changing calibrated scores.

## Input Files
- `all working artifacts`
- `templates/final-report.template.md`

## Output Files
- `reports/final-report.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Do not alter final scores.
- Include missing materials and caveats.
- Keep evidence traceability.

## Failure Modes
- Omitting dissent, hiding gaps, changing chair decisions.

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
