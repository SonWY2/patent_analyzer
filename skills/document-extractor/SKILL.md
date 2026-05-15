# Skill: document-extractor

## Trigger
Extract content from text, PDF, image, or scan inputs.

## Role
Summarize documents and image observations with extraction reliability.

## Input Files
- `input-register.md`
- `raw files`

## Output Files
- `extracted/extraction-log.md`
- `extracted/document-summary.md`
- `extracted/image-observations.md`

## Procedure
1. Read the global rules in `AGENTS.md`.
2. Read the required input files and identify missing prerequisites.
3. Produce the output files using the matching templates where available.
4. Include evidence IDs for any score-bearing or audit-relevant claim.
5. Add a handoff section listing decisions, gaps, and next-step inputs.

## Hard Rules
- Do not infer invisible image content.
- Mark low-confidence OCR.
- Separate quoted/extracted facts from interpretation.

## Failure Modes
- Unreadable files, low image resolution, failed OCR, missing tables/figures.

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
