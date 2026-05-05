# AGENTS Instructions

Scope: entire repository.

- This repository is for pack/connector bundle declarations only.
- Do not add skill manifests, runtime drives, registry cores, MCP server implementations, or API keys.
- Pack manifests should stay minimal and declarative.
- Explicitly declare permissions using `read`, `write`, `draft`, or `append`.
- Put `confirmed_facts`, `assumptions`, `unverified`, and `risks` in scorecards, not in pack manifests.
