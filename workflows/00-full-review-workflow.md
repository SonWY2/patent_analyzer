# Full Review Workflow

## Required Inputs
Patent disclosure, attorney review if available, invention images, architecture diagrams, business plans, Samsung SDS product/technology/roadmap materials, papers, competitor comparisons, and external trend materials.

## Required Outputs
Final report at `working/{case}/reports/final-report.md` plus all intermediate artifacts.

## 15-Step Procedure

| Step | Purpose | Skill | Reads | Creates | Completion Condition | Handoff |
|---:|---|---|---|---|---|---|
| 1 | Register inputs | `patent-intake` | raw files, user prompt | `input-register.md`, `missing-inputs.md` | all files have IDs, type, source, date/confidentiality if known | file inventory and missing inputs |
| 2 | Extract documents | `document-extractor` | input register, raw files | `extracted/extraction-log.md`, `document-summary.md`, `image-observations.md` | each file has extraction status and confidence | extracted facts and uncertain areas |
| 3 | Generate invention map | `invention-structurer` | extracted summaries | `invention/invention-map.md` | problem, solution, components, effects, claim candidates are mapped | structured invention and gaps |
| 4 | Explore creatively | `creative-expansion` | invention map | `creative/creative-hypotheses.md` | every idea is labeled hypothesis with required evidence | evidence research targets |
| 5 | Research evidence | `evidence-web-researcher` | invention map, hypotheses, provided docs | `evidence/evidence-pack.md`, `missing-evidence.md` | every evidence item has ID, source, claim linkage, confidence | evidence pool |
| 6 | Technical review | `technical-excellence-judge` | invention map, evidence, technical rubric | `score_cards/technical-score-card.md` | itemized /30 score with evidence IDs | provisional technical score |
| 7 | Business review | `business-utilization-judge` | evidence, business rubric | `score_cards/business-score-card.md` | itemized /30 score with evidence IDs | provisional business score |
| 8 | Patentability review | `patentability-judge` | invention map, attorney review, prior art evidence | `score_cards/patentability-review.md` | novelty/inventive-step/claim risks recorded | technical cap risks |
| 9 | Competitor review | `competitor-analyst` | evidence, competitor docs | `council/competitor-review.md` | comparison matrix completed or gap recorded | max-score gate status |
| 10 | Product roadmap review | `product-roadmap-analyst` | SDS docs, evidence | `council/product-roadmap-review.md` | product/roadmap fit and gaps recorded | business cap risks |
| 11 | Challenge high claims | `devil-advocate` | all score cards and evidence | `council/devil-advocate.md` | high-score claims have substantive challenges | unresolved challenge list |
| 12 | Audit evidence | `evidence-auditor` | evidence, score cards, council docs | `council/evidence-audit.md` | each score-bearing claim is supported/partial/unsupported | excluded evidence list |
| 13 | Apply score caps | `score-chair` | audit, cap rules, max gate | `council/score-calibration.md` | caps and max-score gates applied | final score candidates |
| 14 | Chair synthesis | `score-chair` | all review artifacts | `council/chair-synthesis.md` | final rationale and missing materials are clear | report-ready conclusion |
| 15 | Generate report | `report-writer` | all artifacts, final template | `reports/final-report.md` | committee-ready report completed | final deliverable |

## Completion Checklist
- [ ] Creative hypotheses are separated from score-bearing evidence.
- [ ] Evidence Auditor excluded unsupported evidence.
- [ ] Devil's Advocate challenged any maximum-score candidate.
- [ ] Score Chair applied all relevant caps.
- [ ] Final report names missing materials and max-score blockers.
