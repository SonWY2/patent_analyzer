# Skill: patent-intake

## Trigger
Register new patent review cases and inventory input materials.

## Role
Create case metadata, file IDs, missing-input list, and handoff notes.

## Input Files
- `raw input files`
- `user prompt`

## Output Files
- `input-register.md`
- `missing-inputs.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Do not interpret technical merit.
- Record source/date/confidentiality when available.
- Flag missing business, roadmap, competitor, attorney, paper, and trend evidence.

## Failure Modes
- Missing or ambiguous files, unknown source, duplicate versions.

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
