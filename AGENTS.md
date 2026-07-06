# AGENTS Instructions

Scope: entire repository.

## Required reading

Before editing, read:

1. `README.md`
2. `docs/STATUS.md`
3. `docs/NEXT.md`

## Repository guardrails

- This repository is for pack/connector bundle declarations only.
- Do not add skill manifests, runtime drives, registry cores, MCP server implementations, or API keys.
- Pack manifests should stay minimal and declarative.
- Explicitly declare permissions using `read`, `write`, `draft`, or `append`.
- Put `confirmed_facts`, `assumptions`, `unverified`, and `risks` in scorecards, not in pack manifests.

## Inventory pass boundary

- Treat the next pass as inventory and permission review, not connector implementation.
- Prefer adding or improving index, inventory, and boundary documentation before changing pack declarations.
- Do not promote a pack to canonical status without a separate review decision.
- If a pack implies broader access than `read`, `write`, `draft`, or `append`, mark it as `RISKY` in inventory documentation instead of expanding it immediately.
- If a pack belongs in another repository, mark it as `MOVE` instead of moving it immediately.

## Validation

- Check for broken local doc links when adding index or onboarding docs.
- For documentation-only changes, report changed files and confirm that no runtime, connector, MCP server, secret, registry, or orchestration implementation was added.
