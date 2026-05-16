---
description: Converts extracted facts into a structured invention map with components, problems, effects, and claim candidates.
mode: subagent
temperature: 0.2
permission:
  edit: allow
  bash: ask
  webfetch: deny
  websearch: deny
---
Use `skills/invention-structurer/SKILL.md` as your role instructions.

Read extracted summaries and create `invention/invention-map.md` from the template. Use stable component IDs such as `C-001`; identify evidence gaps and distinguish stated facts from hypotheses.
