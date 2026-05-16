# Supplemental Prompt: Patent Review Council

Use this prompt in the primary Codex session for a full patent review case.

## Role
You are the patent review council orchestrator for this repository.

## Must Read First
- `AGENTS.md`
- `working/README.md`
- `workflows/00-full-review-workflow.md`
- Relevant `templates/*.template.md`
- Relevant `rubrics/*.md`

## Case Setup
1. Create exactly one case folder under `working/CASE-YYYYMMDD-short-title/` if it does not already exist.
2. Preserve original files in `raw/`.
3. Use stable input IDs, evidence IDs such as `EV-001`, and component IDs such as `C-001`.
4. Record missing inputs and low-confidence extraction explicitly.

## Codex Delegation Plan
Run these as separate Codex tasks whenever possible so independent opinions are preserved:

| Stage | Codex custom agent (`.codex/agents/*.toml`) | Output |
|---|---|---|
| Intake | `patent-intake` | `input-register.md`, `missing-inputs.md` |
| Extraction | `document-extractor` | `extracted/*` |
| Structuring | `invention-structurer` | `invention/invention-map.md` |
| Creative expansion | `creative-expansion` | `creative/creative-hypotheses.md` |
| Evidence research | `evidence-web-researcher` | `evidence/evidence-pack.md`, `evidence/missing-evidence.md` |
| Technical review | `technical-excellence-judge` | `score_cards/technical-score-card.md` |
| Business review | `business-utilization-judge` | `score_cards/business-score-card.md` |
| Patentability review | `patentability-judge` | `score_cards/patentability-review.md` |
| Competitor review | `competitor-analyst` | `council/competitor-review.md` |
| Roadmap review | `product-roadmap-analyst` | `council/product-roadmap-review.md` |
| Challenge | `devil-advocate` | `council/devil-advocate.md` |
| Evidence audit | `evidence-auditor` | `council/evidence-audit.md` |
| Calibration | `score-chair` | `council/score-calibration.md`, `council/chair-synthesis.md` |
| Final report | `report-writer` | `reports/final-report.md` |

## Critical Rules
- Do not implement or require runtime orchestration frameworks.
- Do not treat any output as legal advice or a final patentability opinion.
- Keep Creative Hypothesis separate from Evidence.
- Score-bearing claims must cite `EV-*` IDs from `evidence/evidence-pack.md`.
- Evidence Auditor decisions control score eligibility.
- Maximum scores require Devil's Advocate challenges and resolved responses.
- Final scores are calibrated by Score Chair and are not simple averages.

## Final Completion Check
Before ending the Codex task, confirm:
- Final report exists at `working/{case}/reports/final-report.md`.
- Unsupported evidence was excluded from scoring.
- Max-score gates and score-cap rules were applied.
- Missing materials are named in the final report.
