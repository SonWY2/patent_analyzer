# Codex Patent Review Workflow

This folder uses Codex's TOML-based project configuration format.

## Loaded by Codex

- `.codex/config.toml` sets project-scoped subagent limits for trusted checkouts.
- `.codex/agents/*.toml` defines project-scoped custom subagents. Each TOML file includes `name`, `description`, and `developer_instructions`.

## Supplemental Prompt

- `.codex/prompts/patent-review-council.md` is a reusable kickoff prompt for a primary Codex session. It is documentation/prompt material, not a Codex config file.

## Recommended Codex Flow

1. Create or select a case folder under `working/CASE-YYYYMMDD-short-title/` and place source materials in `raw/`.
2. Start Codex at the repository root so it can read `AGENTS.md` and `.codex/config.toml`.
3. Use `.codex/prompts/patent-review-council.md` as the primary session prompt.
4. Delegate independent work to TOML custom agents in `.codex/agents/`.
5. Merge outputs back into the same case folder before running Evidence Auditor, Score Chair, and Report Writer tasks.

## Best Subagent Candidates

Use separate Codex tasks for work that must remain independent before calibration:

- `technical-excellence-judge`
- `business-utilization-judge`
- `patentability-judge`
- `competitor-analyst`
- `product-roadmap-analyst`
- `devil-advocate`
- `evidence-auditor`
- `score-chair`

The `score-chair` task must run after Evidence Auditor. The `report-writer` task must run after Score Chair.
