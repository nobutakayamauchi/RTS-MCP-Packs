# RTS MCP Packs Repository Position

## What this repository is

RTS MCP Packs is the connector-bundle layer.

This repository groups external tools into purpose-shaped packs that can support RTS Skills.

A pack is not a business workflow.
A pack is not the trust core.
A pack is not the runtime.

A pack is a structured bundle of external capabilities.

## Core responsibility

RTS MCP Packs is responsible for:
- grouping MCP tools into meaningful bundles
- declaring supported tools and permissions
- declaring environment and auth expectations
- mapping packs to compatible skills
- separating read-only and write-enabled usage where needed
- reducing connector sprawl into reusable units

## Non-responsibility

RTS MCP Packs does not:
- define canonical trust records
- decide business intent on its own
- own orchestration schedules or routing
- replace skill definitions
- become the execution log source of truth

## Design stance

Packs should be organized by work support, not by arbitrary tool accumulation.

Preferred examples:
- Dev Pack
- Knowledge Pack
- Biz Pack
- Research Pack
- Infra Pack

A pack exists to support a class of work.
It should not become a dumping ground of unrelated connectors.

## Dependency stance

Packs may depend on:
- external MCP-compatible tools or services
- environment configuration
- permission declarations

Packs should stay as portable as possible and should avoid embedding runtime-specific logic when that logic belongs in a drive layer.

## Expected artifacts

Typical artifacts in this repository include:
- pack manifests
- tool bundle definitions
- permission maps
- environment requirement docs
- compatibility maps
- read/write policy notes
- example pack compositions
