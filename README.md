# Patent Review Council Skill Pack

Markdown-first multi-agent workflow pack for patent review. It is designed for coding-agent tools that read repository instructions and Markdown skills, including Codex, Claude Code, Gemini CLI, and OpenCode.

## Quick Start
1. Put input files in a case folder under `working/CASE-YYYYMMDD-short-title/raw/`.
2. Read `workflows/00-full-review-workflow.md`.
3. Execute each step with the named `skills/*/SKILL.md`.
4. Use `templates/*.template.md` for every artifact.
5. Apply `rubrics/max-score-gate.md` and `rubrics/score-cap-rules.md` before writing the final report.

## Core Principle
Creative ideas may guide research, but final scores must be constrained by objective evidence.

## Directory Map
- `workflows/`: execution procedures.
- `skills/`: role-specific agent instructions.
- `rubrics/`: scoring, cap, and max-score gate rules.
- `schemas/`: machine-readable artifact contracts.
- `templates/`: human-readable output formats.
- `working/`: case execution artifacts.

## OpenCode Usage

This repository includes project-level OpenCode configuration:

- `opencode.json` loads `AGENTS.md` and selects `patent-review-council` as the default primary agent.
- `.opencode/agents/patent-review-council.md` is the orchestrator for the full review workflow.
- `.opencode/agents/*.md` defines the specialized subagents that mirror the existing `skills/*/SKILL.md` roles.
- `.opencode/commands/patent-review.md` starts or continues a full case workflow from OpenCode.

Recommended OpenCode flow:

1. Place source materials in `working/CASE-YYYYMMDD-short-title/raw/`, or ask the council agent to create a new case folder.
2. Run the `patent-review` command, or ask `@patent-review-council` to execute `workflows/00-full-review-workflow.md`.
3. Let the council agent delegate independent reviews to subagents before debate, evidence audit, and score calibration.
4. Review the final report at `working/{case}/reports/final-report.md`.

Use subagents especially for independent technical, business, patentability, competitor, product-roadmap, Devil's Advocate, Evidence Auditor, and Score Chair work. These roles are intentionally separated so score-bearing claims remain evidence-bound and calibrated rather than averaged.

