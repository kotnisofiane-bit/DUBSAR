# Changelog

All notable public repository and distribution changes will be recorded here.

## 2026-07-30

### Historical Marketplace surface retired

- removed the active `.claude-plugin/marketplace.json` staging manifest;
- removed the vendored `plugins/scribe/` executable runtime from the active
  tree;
- replaced public installation and integrity instructions with a
  non-installable retirement record;
- preserved version `0.11.1`, its source pin and aggregate hash in a
  non-executable tombstone;
- moved the exact historical private-beta licence into that tombstone and
  removed it as the current repository-root licence;
- added `RIGHTS.md` to record that no public software licence is currently
  selected and that third-party licences remain unaffected;
- kept future Marketplace publication behind a new provenance, licence,
  installation and explicit Human GO review.

No public package, release or installation command was created by this change.

## Earlier public realignment

### Current positioning refresh

- aligned the repository with the current `dubsar.ai` website;
- presented two distinct entry paths: the DUBSAR private-beta product and DUBSAR Audit professional service;
- separated product-readiness labels from professional-service availability;
- documented launch-readiness and agent-governance audit mandates;
- added English and French public entry-point documentation;
- clarified that audits are remote, bounded, read-only by default and human-validated.

## Unreleased — DUBSAR public realignment R2

### Changed

- public product name and current-facing copy standardized on DUBSAR;
- public positioning broadened from a Claude Code-only product to a host-adapter governance layer for long-running AI coding projects;
- Claude Code retained as the first supported integration;
- Codex, Cursor and other coding-agent adapters classified as future direction, not current availability;
- public architecture aligned with host adapter → local Bridge/runtime → private Backend → private Core → human-facing cockpit;
- canonical session, worktree, process, evidence and Human Gate responsibilities clarified;
- internal one-session and two-session Windows technical proofs reflected without claiming public beta availability;
- Windows identified as the first controlled private-beta target;
- Linux classified as later validation and macOS as unannounced pending feasibility;
- speculative Scribe Launcher and Eyes of SCRIBE product brands removed from current product surfaces;
- legacy internal `scribe` identifiers retained only where required for compatibility;
- `WHY_SCRIBE.md` replaced by `WHY_DUBSAR.md`.

### Historical Marketplace staging (retired 2026-07-30)

- the repository contained an unpublished Marketplace staging surface;
- the Marketplace was not activated or announced;
- no supported public installation command is active;
- plugin `0.11.1` was an earlier staging pin, not a final publication candidate;
- the manifest and vendored runtime were later retired from the active tree.

### Added or refreshed

- host-independent product definition;
- explicit multi-session public architecture;
- Windows-first installation boundary;
- platform status for Windows, Linux and macOS;
- distinction between internal technical proof and external product validation;
- adapter direction for Codex, Cursor and other coding agents.

### Not published

- no Marketplace activation or announcement;
- no public installation command;
- no release or tag;
- no repository rename;
- no Linux or macOS support claim;
- no operational Codex or Cursor support claim;
- no private Core or Backend implementation exposed.

```text
product generally available: no
public beta: no
marketplace-ready: no
```

## Legacy history

Earlier repository history documents the project under SCRIBE and Scribe Builder. Git history is intentionally preserved and should not be rewritten. Legacy names are not current public product brands.
