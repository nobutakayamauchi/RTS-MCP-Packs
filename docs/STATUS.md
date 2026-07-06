# RTS-MCP-Packs Status

Status: PARTS / CONNECTOR-PACKS / INVENTORY NEEDED

RTS-MCP-Packs is the declarative connector pack definition shelf for the RTS ecosystem.

It is a component repository, not RTS core.

It is not RTS-Skills.

It is not RTS-Hermes-Drive.

It is not an MCP server implementation repository.

It is not a runtime execution engine.

## Current Position

This repository should hold minimal pack and connector bundle declarations that describe how future operator environments may connect to tools, data sources, or workflows.

Pack definitions should stay declarative.

Permissions should be explicit.

Secrets, API keys, runtime implementations, and connector internals do not belong here.

Allowed by default:

- document pack definitions
- add concise pack manifests
- clarify permission declarations
- improve pack indexing
- organize connector bundle documentation
- document pack boundaries and risks
- keep pack declarations minimal and inspectable

Prohibited by default:

- adding MCP server implementations
- adding runtime execution engines
- adding API keys or secrets
- adding connector internals
- importing RTS-Skills manifests as pack bodies
- importing Hermes Drive orchestration internals
- importing Talent Registry internals
- importing Signal Feed registry internals
- turning this repository into RTS core
- broad refactors without an inventory decision

## Permission Vocabulary

Use explicit permission labels when documenting pack access:

- `read`
- `write`
- `draft`
- `append`

Any broader permission should require a separate decision record.

## Boundary

RTS defines the protocol.

RTS-Skills holds reusable job-shaped skill definitions.

RTS-Hermes-Drive may hold orchestration bridge material.

RTS-AGE may execute or prepare implementation artifacts.

RTS-MCP-Packs should remain the declarative connector pack shelf.

## Minimum Alive Definition

This repository is considered Minimum Alive when:

1. Its role as a declarative connector pack shelf is explicit.
2. Its boundaries from skills, runtime, server implementation, and orchestration repositories are clear.
3. Permission vocabulary is documented.
4. Its next inventory pass is documented.
5. No runtime, server, connector, or secret material is added by the rescue documentation itself.

## Current Decision

Keep this repository.

Treat it as a parts shelf for minimal MCP connector pack declarations.

Do not expand it into runtime, server, registry, or orchestration implementation without a separate decision record.
