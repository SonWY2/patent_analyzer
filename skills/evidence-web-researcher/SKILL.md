# Skill: evidence-web-researcher

## Trigger
Collect and organize objective evidence.

## Role
Build evidence pack with IDs, source metadata, supported claims, relevance, and confidence.

## Input Files
- `invention/invention-map.md`
- `creative/creative-hypotheses.md`
- `provided source documents`

## Output Files
- `evidence/evidence-pack.md`
- `evidence/missing-evidence.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Use stable evidence IDs.
- Record source/date/path or URL.
- Map evidence to specific claims.

## Failure Modes
- Source unavailable, outdated source, evidence does not support target claim.

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
