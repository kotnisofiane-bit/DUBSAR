# Public Realignment Audit — R3

Date: 29 July 2026

## Scope

This review realigns the public DUBSAR documentation with the current product direction:

- portal-first audit;
- business automations and AI agents;
- deterministic controls and private canonical state;
- bounded Hermes roles;
- explicit human review;
- continuous governance after the initial audit;
- future local Node and administration desktop;
- developer adapters as secondary experiments.

It does not publish private repositories, certify the product, change the private Core or complete the pending licence audit.

## Previous mismatch

The public repository still presented:

- Claude Code as the first and primary product;
- a Windows desktop beta as the main access path;
- developer-project governance as the central customer problem;
- audit mainly as a manually operated professional service;
- a future coding-agent Marketplace as the public distribution goal.

Those foundations remain relevant experiments, but they no longer describe the first customer-facing product.

## Current product truth

The first intended journey is:

```text
bounded authorized sources
→ immutable evidence snapshot
→ deterministic controls
→ specialized Hermes roles
→ human review
→ traceable report
```

The first Rule Pack under consolidation is **Automation Coherence**, covering:

1. duplicate consequences without an attributable idempotency boundary;
2. actions incompatible with observed business state;
3. missing version, rule or expected human-validation evidence in the connected scope.

The current proof boundary is:

```text
deterministic synthetic-fixture controls: validated internally
recorded API audit path: internal evidence exists
complete portal browser journey: not yet proved
live connectors: not yet proved
continuous enforcement: roadmap
local Node / administration desktop: prototype and roadmap
production availability: no
```

## Architecture boundary

- The portal is the primary user surface.
- The deterministic orchestrator controls transitions.
- The private Core owns canonical state and authority.
- Hermes supplies bounded, non-authoritative roles.
- Human review is required for final dispositions.
- The report preserves evidence, decisions and limitations.
- A future Node submits bounded evidence but does not bypass Core or human authority.

## AI Act boundary

DUBSAR may help document governance-relevant elements such as traceability, provenance, retained evidence and human oversight.

It does not:

- certify AI Act compliance;
- provide legal advice;
- automate a legal verdict;
- replace a client-specific compliance assessment.

## Developer-adapter boundary

Claude Code, Codex and Cursor adapters remain relevant product experiments.

The visible Claude Marketplace material is historical staging and must not be presented as installable or supported. Publication requires separate licence, integrity, compatibility and user-journey validation.

## Public repository boundary

The public repository may contain:

- public product documentation;
- high-level architecture;
- synthetic examples;
- approved contracts and diagrams;
- security, privacy and integrity boundaries;
- explicitly approved thin adapters.

Technical implementation repositories remain private. Their current documentation includes legacy branding, internal topology, deployment detail and unreconciled third-party attribution.

## Files realigned in R3

Primary product documents:

- `README.md`;
- `README.fr.md`;
- `WHY_DUBSAR.md`;
- `WHY_NOT_JUST_AGENTS.md`;
- `PRODUCT_SURFACES.md`;
- `ARCHITECTURE.md`;
- `STATUS.md`;
- `ROADMAP.md`;
- `AUDIT.md`;
- `AUDIT.fr.md`;
- `FAQ.md`.

Trust and distribution boundaries:

- `INSTALLATION.md`;
- `MARKETPLACE.md`;
- `SECURITY.md`;
- `PRIVACY.md`;
- `INTEGRITY.md`;
- `.claude-plugin/marketplace.json`.

## Merge gate and follow-up decisions

This public realignment must not merge while the active Marketplace manifest
and historical plugin subtree remain a technically installable surface with
unreconciled licence metadata. The publication gate must resolve that boundary
by either:

- removing or quarantining the distribution surface from `main`; or
- completing licence, provenance, compatibility and publication approval for
  an intentionally supported adapter.

Separate work is also required to:

- reconcile third-party notices;
- prove the complete internal browser E2E;
- validate portal authentication, retention and deletion;
- lock down external portal access;
- update repository description and topics;
- update the public profile;
- decide what to do with the public `scribe-demo-public` legacy name;
- publish only after human review of the final diff.

## Verdict

This documentation branch can align the public product story without claiming that the product is already ready.

It should be reviewed as a copy and boundary change. It must not be used as evidence that the portal, connectors, desktop or continuous governance are complete.
