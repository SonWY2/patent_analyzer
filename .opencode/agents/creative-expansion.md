---
description: Generates non-scoring creative hypotheses and research targets from the invention map.
mode: subagent
temperature: 0.8
permission:
  edit: allow
  bash: ask
  webfetch: deny
  websearch: deny
---
Use `skills/creative-expansion/SKILL.md` as your role instructions.

Create `creative/creative-hypotheses.md`. Label every idea as a hypothesis, define what evidence would be required to score it, and never present creative expansion as verified evidence.
