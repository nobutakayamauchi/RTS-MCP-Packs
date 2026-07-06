# RTS-MCP-Packs Next Actions

The next goal is an inventory pass, not connector implementation.

## Next Tasks

1. List existing pack and connector bundle declarations.
2. Identify which packs are ready, draft, stale, duplicate, risky, or misplaced.
3. Confirm permission declarations for each pack.
4. Confirm whether each pack is purely declarative.
5. Check local documentation links.
6. Decide which pack definitions should remain here and which belong in adjacent repositories.

## Suggested Follow-up Files

```text
docs/inventory/pack_inventory.md
docs/contracts/pack_manifest_contract.md
docs/relations/adjacent_repo_boundaries.md
```

## Inventory Categories

Use these labels during the next pass:

- READY: usable as a minimal declarative pack definition
- DRAFT: useful but incomplete
- STALE: likely outdated or superseded
- DUPLICATE: overlaps another pack
- RISKY: permissions or scope need review
- MOVE: belongs in another repository
- ARCHIVE: preserve for history only

## Permission Review

Each pack should explicitly describe whether it needs:

- `read`
- `write`
- `draft`
- `append`

If a pack implies broader access, mark it as `RISKY` and do not expand it until reviewed.

## Do Not Do Yet

Do not:

- add MCP server implementation code
- add connector internals
- add API keys, tokens, or secrets
- add runtime execution code
- import RTS-Skills manifests as pack bodies
- import Hermes Drive orchestration internals
- rewrite all manifests at once
- promote a pack to canonical status without review

## Next Recommended Task

Create `docs/inventory/pack_inventory.md`.

That file should list each known pack or connector bundle with:

1. name
2. path
3. purpose
4. status label
5. permission labels
6. expected boundaries
7. adjacent repo relation
8. next smallest safe action
