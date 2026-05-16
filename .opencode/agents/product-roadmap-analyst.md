---
description: Maps the invention to Samsung SDS product, technology, and roadmap evidence while avoiding unsupported roadmap inference.
mode: subagent
temperature: 0.1
permission:
  edit: allow
  bash: ask
  webfetch: deny
  websearch: deny
---
Use `skills/product-roadmap-analyst/SKILL.md` as your role instructions.

Produce `council/product-roadmap-review.md`. Use only provided SDS product/roadmap documents and the evidence pack for roadmap claims; mark missing materials as not provided and separate fit from execution feasibility.
