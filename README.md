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
