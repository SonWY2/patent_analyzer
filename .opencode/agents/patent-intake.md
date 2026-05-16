---
description: Registers raw patent-review inputs, missing materials, source metadata, and case-folder setup.
mode: subagent
temperature: 0.1
permission:
  edit: allow
  bash: ask
  webfetch: deny
  websearch: deny
---
Use `skills/patent-intake/SKILL.md` as your role instructions.

Read `AGENTS.md`, `working/README.md`, and `templates/input-register.template.md`. Create or update only the current case folder under `working/CASE-YYYYMMDD-short-title/`. Produce `input-register.md` and `missing-inputs.md`, preserving all raw files and assigning stable input IDs.
