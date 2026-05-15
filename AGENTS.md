# Patent Review Council Agent Rules

## Mission
Create committee-ready patent review reports from invention disclosures, attorney reviews, images, architecture diagrams, business documents, Samsung SDS product/technology/roadmap materials, papers, competitor comparisons, and external technology-trend materials.

## Non-Goals
- Do not implement or require LangGraph, AutoGen, CrewAI, or any runtime orchestration framework.
- Do not treat any output as legal advice or a final patentability opinion.
- Do not infer confidential Samsung SDS roadmap facts unless a provided source supports them.

## Global Principles
1. Separate **Creative Hypothesis** from **Evidence**.
2. Creative expansion is encouraged, but score-bearing claims must be limited by supported evidence.
3. Multiple personas must evaluate independently before debate and calibration.
4. Final scores are not averages; the Score Chair applies evidence quality, max-score gates, and score caps.
5. A maximum score is forbidden unless Devil's Advocate challenges have been made and resolved.
6. Evidence Auditor decisions control score eligibility: `unsupported` evidence is excluded.
7. Record extraction reliability and missing information for image/PDF inputs.
8. The final report must be clear enough for direct use in a human patent review committee.

## Working Directory Rules
Create one case folder under `working/CASE-YYYYMMDD-short-title/`. Store intermediate artifacts in the matching subdirectories documented in `working/README.md`. Use stable evidence IDs such as `EV-001` and component IDs such as `C-001`.

## Evidence Rules
Each score-bearing statement must cite evidence IDs from `evidence/evidence-pack.md`. If a claim is based on agent reasoning, label it as `hypothesis` and do not use it for scoring until verified.

## Scoring Rules
Technical Excellence and Business Utilization are each scored out of 30. Apply `rubrics/max-score-gate.md` and `rubrics/score-cap-rules.md` before finalizing scores.

## Final Report Rules
The final report must include scores, score rationale, objective evidence table, independent opinions, Devil's Advocate challenges, Evidence Audit results, score calibration, maximum-score eligibility, and missing materials.
