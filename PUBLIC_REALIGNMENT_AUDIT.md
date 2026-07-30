# Public Realignment Audit — R2

## Scope

This audit reviews the public repository against the current DUBSAR product direction after the internal one-session and two-session Windows technical proofs.

It covers public positioning, architecture, product surfaces, platform claims, Marketplace staging, status, roadmap, FAQ and compatibility naming.

It does not publish or independently audit the private Core implementation.

---

## Executive verdict

The original public doctrine contained a strong foundation:

- decision memory is different from conversation history;
- agents should not self-validate;
- evidence matters more than persuasive explanation;
- protected movement requires explicit human authority;
- replay and fail-closed boundaries matter;
- the proprietary Core should remain private.

The main defect was the public product story.

The repository was originally framed around:

- SCRIBE or Scribe Builder as the public brand;
- Scribe Launcher as a speculative product surface;
- Eyes of SCRIBE as a separate cockpit direction;
- plugins and MCP as hypothetical future delivery forms;
- documentation-only publication;
- no concrete multi-session product claim.

That story no longer matches the product trajectory.

---

## Current product truth

DUBSAR is one governance product with host-specific adapters.

```text
Coding agent
  → DUBSAR host adapter
  → local Bridge and runtime
  → private Backend
  → private DUBSAR Core
  → governed project state
  → human-facing cockpit and decision
```

Claude Code is the first supported integration.

The same Core is intended to support future adapters for Codex, Cursor and other coding-agent environments. Those adapters are not currently available.

The user experiences one product called DUBSAR.

---

## Technical proof versus product availability

Internal Windows technical proofs have completed:

- one real governed Claude Code session;
- two real sessions linked to the same canonical Mission;
- distinct identities, processes and worktrees;
- separated evidence;
- explicit conflict handling without silent overwrite;
- Human Gate and single-use authorization behavior;
- restart reconciliation.

These proofs establish a serious technical substrate.

They do not establish:

- a supported public installation;
- an autonomous external tester journey;
- Linux or macOS support;
- operational Codex or Cursor integrations;
- commercial or production readiness.

The next product-validation target is a reproducible Windows private-beta journey without hidden expert intervention.

---

## Public naming classification

### Current public product name

- DUBSAR.

### Current public surfaces

- DUBSAR for Claude Code;
- DUBSAR Desktop and local runtime;
- DUBSAR cockpit.

These are surfaces of one product, not separate brands.

### Obsolete current-facing product names

- SCRIBE;
- Scribe Builder;
- Scribe Launcher;
- Eyes of SCRIBE.

These names may remain in Git history or explicit legacy archives, but must not describe the current product.

### Temporary technical compatibility identifiers

- private repository names;
- `scribe-bridge`;
- `scribe-mcp`;
- `/scribe-*` commands;
- `scribe.*` MCP tools;
- `SCRIBE_*` environment variables;
- historical routes, schemas and storage paths.

These identifiers do not create a second product. They should be migrated only through tested compatibility work.

---

## Product responsibility model

### Coding-agent host

Owns native intelligence, editing, tools, tests, sub-agents and worktrees.

### Host adapter

Propagates native session identity, exposes bounded DUBSAR surfaces and connects to the local runtime.

### Local Bridge

Provides bounded local transport and orchestration without owning canonical Mission state.

### DUBSAR Desktop

Provides local runtime, process/worktree mechanics and human-facing controls.

### Private Backend

Protects the private boundary and remains the only supported writer to canonical Core state.

### Private Core

Owns Mission, decisions, contracts, canonical sessions, evidence relationships, audit, Human Gates and replay.

### Runner

Produces mechanical evidence such as snapshots, diffs, tests and hashes.

### Cockpit

Displays and controls governed state without becoming an approval authority.

---

## Platform claims

### Windows

First controlled private-beta target. Product installation and the independent tester journey remain in preparation.

### Linux

Planned for later validation. No support announcement yet.

### macOS

Not announced. Packaging, signing, permissions and runtime feasibility must be evaluated first.

The public repository must not imply cross-platform support from code portability or CI alone.

---

## Marketplace decision

The public repository remains the home for DUBSAR documentation, doctrine and
public distribution status. It does not currently contain or advertise an
installable Claude Code Marketplace package.

The historical staging manifest and vendored runtime were retired from the
active tree on 2026-07-30. Any future package location is a later distribution
decision, not a commitment made by this audit.

---

## Retired Marketplace staging record

The repository previously contained a vendored plugin runtime from:

```text
scribe-claude-code-plugin@c2878313198aceccac078bf9446c5ab45751e424
version 0.11.1
```

This was an earlier staging pin, not a final publication candidate. Its
executable manifest and runtime are no longer present in the active tree. A
non-executable tombstone preserves the source pin and aggregate hash.

Any future package must start from a newly approved commit and receive new
integrity, dependency, licence and installation review.

---

## Publication blockers

Before any future Marketplace publication or announcement:

- complete the current-facing DUBSAR copy;
- remove obsolete product-brand references from navigation and primary visuals;
- stabilize the Windows tester journey;
- select the final plugin commit and version;
- generate a minimal package from that exact pin;
- regenerate integrity hashes;
- pass strict Marketplace and plugin validation;
- verify installation, update, rollback and removal on Windows;
- verify Privacy and Security documents against the implemented data flow;
- confirm public security and licensing contacts are monitored;
- decide the final public plugin id;
- decide whether the repository is renamed before publication;
- obtain a separate explicit Human GO to activate and announce the Marketplace.

Linux and macOS are not automatic blockers for an initial Windows-only controlled beta.

---

## Files realigned in R2

Current-facing documents updated:

- `README.md`;
- `WHY_DUBSAR.md`;
- `PRODUCT_SURFACES.md`;
- `ARCHITECTURE.md`;
- `STATUS.md`;
- `ROADMAP.md`;
- `FAQ.md`;
- `MARKETPLACE.md`;
- `INSTALLATION.md`;
- `CHANGELOG.md`;
- the non-executable historical Marketplace tombstone.

Legacy `WHY_SCRIBE.md` was removed from the branch.

---

## Remaining public work

- redraw canonical DUBSAR diagrams;
- migrate or archive legacy diagram and RFC branding;
- add real product captures only when they reflect the approved product build;
- update GitHub repository description, topics, website link and social preview;
- decide and execute repository rename under separate Human GO;
- re-vendor the final plugin runtime after Windows stabilization;
- merge only after a separate human review and GO.

---

## Canonical status

```text
DUBSAR PUBLIC REPOSITORY REALIGNMENT R2 — REVIEW BRANCH
WINDOWS CONTROLLED PRIVATE BETA — IN PREPARATION
INTERNAL ONE-SESSION TECHNICAL PROOF — COMPLETED
INTERNAL TWO-SESSION TECHNICAL PROOF — COMPLETED
EXTERNAL INSTALLATION AND USABILITY PROOF — PENDING
HISTORICAL MARKETPLACE SURFACE — RETIRED FROM ACTIVE TREE
FINAL PUBLIC PLUGIN PIN — NOT SELECTED
REPOSITORY — NOT RENAMED
NO PRIVATE CORE PUBLISHED
not commercial-ready
not beta-ready
not marketplace-ready
```
