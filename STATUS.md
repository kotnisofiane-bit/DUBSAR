# Status

DUBSAR is an active governance and audit system with three distinct product
surfaces:

1. an automated audit portal;
2. a bounded professional audit service;
3. a private-beta product for software projects built with coding agents.

They share one evidence and human-authority doctrine, but they do not have the same delivery model or maturity level.

## Current status at a glance

| Surface | Current status |
|---|---|
| Automated audit portal | Under construction and validation; coming soon, not publicly available |
| Professional DUBSAR Audit | Available on request |
| DUBSAR for Claude Code | Functional controlled private beta being finalized |
| External coding-agent beta access | Selective, invitation only, Windows first |
| Public Claude Code Marketplace | Retired from the active tree; no public package available |
| Continuous governance / DUBSAR Node | Separate scoped deployment path; not generally available |
| Codex / Cursor adapters | Future direction, not currently available |
| Private DUBSAR Core | Proprietary, under active development, not distributed here |

These statuses must not be conflated.

---

## 1. Automated audit portal

The public [DUBSAR audit page](https://dubsar.ai/audit) is the current commercial
entry point. The automated portal itself is under construction and validation.

Its intended journey is:

1. define a bounded perimeter;
2. identify the automations, period and authorized sources;
3. connect available events without inventing causality;
4. surface inconsistencies, uncertainty and missing information;
5. let the designated owner classify the findings;
6. produce a report that keeps evidence, limitations and validations connected.

The portal is not yet presented as publicly accessible. It will be announced
when its construction and validation boundary supports a controlled public
opening.

The current status does not imply that:

- every connector or client environment is supported;
- every automation can be fully reconstructed;
- an inconsistency is automatically a confirmed failure;
- the portal produces a legal or regulatory compliance verdict;
- the portal has autonomous authority over client systems;
- production-grade availability has been established for every use case.

The target is a clear first result with explicit coverage and human validation.

[Audit overview](https://dubsar.ai/audit)

---

## 2. Professional DUBSAR Audit

Professional DUBSAR Audit is available on request.

It is a bounded engagement operated by Sofiane with:

- an agreed mandate;
- explicitly authorized sources;
- read-only access by default;
- DUBSAR evidence, contradiction and decision records;
- human classification and review;
- a professional report and evidence register.

The primary audit mandates are:

- **launch readiness** — is the product genuinely ready to open to users?
- **agent governance** — can the team explain and verify how the project was built and approved?

A professional audit is not the same as an automated portal diagnostic.

Each engagement requires explicit agreement on:

- scope;
- permissions;
- sources;
- access limitations;
- retention;
- timing;
- price.

No final conclusion is delivered without human review.

[Professional audit method](AUDIT.md) · [Request support on Malt](https://www.malt.fr/profile/sofianekotni)

---

## 3. DUBSAR for coding agents

DUBSAR for coding agents is a governance layer for long-running, multi-session software projects assisted by AI coding agents.

Claude Code is the first integration and the current engineering focus.

The current private-beta product combines:

- a thin Claude Code host adapter;
- a local Bridge;
- DUBSAR Desktop and its local runtime;
- a protected Backend;
- a private DUBSAR Core;
- persistent Mission and decision memory;
- canonical session identity;
- evidence boundaries;
- contradiction handling;
- explicit Human Gates;
- a human-facing cockpit.

Internal Windows proofs have completed:

- one real governed Claude Code session;
- two sessions linked to one canonical Mission;
- distinct identities, processes and worktrees;
- separated evidence;
- explicit conflict handling;
- single-use authorization behavior;
- process control;
- restart reconciliation.

These results establish important technical capabilities.

They do not yet establish that an external user can independently install, understand and operate the complete product journey.

The current validation target is a reproducible Windows path from approved installation to:

```text
Mission
    ↓
Governed work
    ↓
Evidence
    ↓
Human Gate
    ↓
Restart and resume
```

External access remains selective and invitation based.

[Product surfaces](PRODUCT_SURFACES.md) · [Request beta access](https://dubsar.ai/early-access)

---

## Continuous governance and DUBSAR Node

Continuous governance is a separate deployment path that may follow an audit when the need is established.

A DUBSAR Node is intended to apply declared controls inside an authorized client environment.

It is not automatically included with:

- a portal diagnostic;
- an audit report;
- access to the coding-agent beta.

A Node must not create its own authority. It can evaluate or apply declared rules only within an agreed perimeter and must surface a Human Gate when protected authorization is required.

No generally available Node installation or enterprise deployment is currently claimed.

---

## Platform and integration status

### Web portal

Under construction and validation. It is not currently presented as publicly
accessible; the public marketing entry point is the
[audit overview](https://dubsar.ai/audit).

This portal status does not change the maturity status of the installable
coding-agent product.

### Windows

First controlled private-beta target for DUBSAR for coding agents.

Packaging and the autonomous external-tester journey are still being finalized.

### Linux

Planned for later validation. No Linux beta is currently announced.

### macOS

Not currently announced. Packaging, signing and runtime behavior remain to be evaluated.

### Claude Code

First coding-agent integration and current engineering focus.

### Codex, Cursor and other agents

Future host-adapter direction. No operational public support is currently claimed.

---

## Public distribution status

This repository is the public documentation and distribution boundary for DUBSAR.

Current distribution status:

- the repository is publicly available as `kotnisofiane-bit/DUBSAR`;
- public doctrine, architecture and bounded examples are available;
- the thin Claude Code adapter is being prepared through a controlled private
  distribution path and is not published in this repository;
- no supported public installation command is active;
- the historical Marketplace manifest and vendored runtime have been retired
  from the active tree;
- no generally available coding-agent product release is claimed;
- the private Core is not distributed here.

The repository can be referenced as public documentation.

It must not be presented as proof that the coding-agent product is already generally installable or production ready.

---

## Claims not made

DUBSAR is not currently presented as:

- a universally supported automation platform;
- a generally available coding-agent product;
- an autonomous approval, merge, release or deployment authority;
- a substitute for client technical authority;
- a certified compliance or security system;
- an operational Codex or Cursor integration;
- a public release of the private Core;
- a guarantee that an audited product is defect-free or secure.

DUBSAR can support evidence organization, traceability and human-oversight documentation relevant to AI Act readiness.

It does not provide legal advice, issue certification or replace a qualified legal or conformity assessment.

---

## Promotion gates

A stronger availability claim requires evidence appropriate to the surface concerned.

### Automated audit portal

Before a broader production-readiness claim:

- critical journeys must be reproducible;
- connector and coverage limits must be explicit;
- findings and reports must remain reviewable;
- errors and unavailable sources must fail visibly;
- human validation must remain enforceable.

### Professional audit

Each engagement requires:

- an agreed mandate;
- explicit source authorization;
- defined retention and permissions;
- human review;
- an agreed deliverable, timing and price.

### Coding-agent product

Before general availability:

- external installation must be reproducible;
- supported Windows versions must be explicit;
- packaging and update behavior must be validated;
- security and privacy boundaries must be reviewable;
- the complete Mission-to-resume journey must be validated by external testers;
- Marketplace publication requires an explicit Human GO.

No stronger claim should be inferred from internal technical proofs alone.
