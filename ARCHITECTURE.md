# Architecture

## Purpose

Registry contracts curated by the 8004 team

## Portfolio role

- Category: External references and mirrors
- Namespace policy: legacy/external
- Repository: https://github.com/Tesseras-Labs/erc-8004-contracts

## Observed baseline signals

- CI workflow present: no
- Test signal present: no
- Detected stack:
- Node.js
- Solidity

## Baseline boundaries

- Define external contracts before internal abstractions.
- Keep state transitions explicit and auditable.
- Prefer additive changes and clear rollback paths.

## Immediate next steps

1. Replace placeholder architecture assumptions with concrete runtime and data-flow diagrams.
2. Document integration contracts and failure modes.
3. Link production runbooks and ownership records once assigned.

## Repository review (2026-02-17)

### Evidence reviewed

- Tracked files: 54
- Detected stack signals: Node.js,TypeScript,Solidity
- CI workflows detected: no
- Test signal detected: yes

### Code surface snapshot

- Top-level code/module directories: contracts/,scripts/
- Likely runtime entrypoints: hardhat.config.ts

### Architecture callouts

Strengths:
- Test-related files or test directory signals are present.
- Code boundaries are partially explicit via top-level module directories.

Gaps and risks:
- No CI workflow detected; merge safety depends on local discipline.

Recommended next step:
- Add a minimal CI lane (lint + unit smoke) and block merges on it.
