# Project Notes for Claude

## Reference Documentation

When working on this project, always consult the official OpenClaw documentation:

- https://docs.openclaw.ai/tools/clawhub — ClawHub registry, publishing, and metadata format
- https://docs.openclaw.ai/tools/skills — SKILL.md structure and frontmatter spec
- https://docs.openclaw.ai/tools/skills-config — skill configuration and openclaw.json

## Key conventions

- `SKILL.md` frontmatter `metadata` must be a **single-line JSON** with the `openclaw` namespace:
  ```
  metadata: {"openclaw": {"requires": {"bins": [...], "env": [...]}, "primaryEnv": "..."}}
  ```
- `name` in SKILL.md frontmatter is the registry package ID (e.g. `sergei-mikhailov-stt`), not a display name
- Display name is the `#` heading in the body of SKILL.md
