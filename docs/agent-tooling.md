# Agent Tooling Usage

This repository includes project-level configuration for OpenCode and Codex-style workflows. This file intentionally keeps tool-specific guidance outside the root `README.md` to reduce merge conflicts with project overview edits.

## OpenCode

- `opencode.json` loads `AGENTS.md` and selects `patent-review-council` as the default primary agent.
- `.opencode/agents/patent-review-council.md` is the orchestrator for the full review workflow.
- `.opencode/agents/*.md` defines the specialized subagents that mirror the existing `skills/*/SKILL.md` roles.
- `.opencode/commands/patent-review.md` starts or continues a full case workflow from OpenCode.

Recommended OpenCode flow:

1. Place source materials in `working/CASE-YYYYMMDD-short-title/raw/`, or ask the council agent to create a new case folder.
2. Run the `patent-review` command, or ask `@patent-review-council` to execute `workflows/00-full-review-workflow.md`.
3. Let the council agent delegate independent reviews to subagents before debate, evidence audit, and score calibration.
4. Review the final report at `working/{case}/reports/final-report.md`.

## Codex

- `.codex/config.toml` is the project-scoped Codex configuration file.
- `.codex/agents/*.toml` contains Codex custom subagent definitions that mirror the existing `skills/*/SKILL.md` roles.
- `.codex/prompts/patent-review-council.md` is a reusable kickoff prompt for the primary Codex session.

Recommended Codex flow:

1. Place source materials in `working/CASE-YYYYMMDD-short-title/raw/`, or create the case folder from a primary Codex session.
2. Start Codex at the repository root so it can load `.codex/config.toml` and `.codex/agents/*.toml`.
3. Use `.codex/prompts/patent-review-council.md` as the primary prompt, then spawn or select separate Codex custom agents for independent technical, business, patentability, competitor, product-roadmap, Devil's Advocate, Evidence Auditor, and Score Chair work.
4. Merge outputs into the same case folder and run the final `report-writer` task.

Use subagents especially for independent technical, business, patentability, competitor, product-roadmap, Devil's Advocate, Evidence Auditor, and Score Chair work. These roles are intentionally separated so score-bearing claims remain evidence-bound and calibrated rather than averaged.
