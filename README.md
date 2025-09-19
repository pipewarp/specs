# pipewarp specs

This repo is used to hold the pipewarp specification schemas for defining state machine contracts for local AI systems.

It also containgits generated types for TypeScript. Python types, probably in pydantic, will be next.

Currently used for GitHub source install and building to an early alpha for wiring and testing.

- **Schemas** are written in [JSON Schema](https://json-schema.org/) and define the core data contracts.
- **Types** are generated for various languages (starting with TypeScript) to make the specs easier to use in real projects.

## Status

**Alpha** — these specs are experimental, incomplete, and subject to change without notice. Expect breaking changes.

## Structure

- `schemas/` — source JSON Schema files
- `types/` — generated types for each language

## Usage

Install directly from GitHub (example for TypeScript):

```bash
pnpm add github:pipewarp/specs
```

Target a specific version with git tag (current version shown):

```bash
pnpm add github:pipewarp/specs#v0.1.0-alpha.0
```

## Development Scripts

Use `json-schema-to-typescript` to generate TypeScript files (already available in GitHub install)

```bash
pnpm gen
```
