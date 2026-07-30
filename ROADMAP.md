# Roadmap

This roadmap describes the current product direction. It is not a delivery guarantee.

DUBSAR is a **portal-first audit and governance product for AI agents and
business automations** with three distinct delivery surfaces today:

- the automated audit portal, coming soon and currently under construction and
  validation;
- the Professional DUBSAR Audit, available on request;
- DUBSAR for Claude Code, a functional controlled private beta being finalized,
  selective and Windows-first.

DUBSAR Node is a separate scoped deployment path and is not generally
available.

The sequence is deliberate:

```text
clean and reconcile the foundation
  -> build and validate the portal end-to-end
  -> validate the portal with bounded external use
  -> add continuous governance through DUBSAR Node
  -> expand connectors and optional host adapters
```

Professional audits and the controlled coding-agent beta progress in parallel
within their own published boundaries. No external portal pilot should replace
the internal end-to-end proof required for a stronger availability claim.

---

## 0. Reconcile the foundation

Current priority:

- reconcile canonical local and GitHub histories;
- preserve recoverable sources before cleanup;
- identify the authoritative version of each component;
- remove duplicate, stale and accidental artefacts from release paths;
- audit dependencies, licences and provenance before redistribution;
- document the public/private boundary;
- keep the private Core and confidential proof material outside the public repository.

Exit criteria:

- every active component has one identified canonical repository and branch;
- retained changes are attributable and reviewable;
- licence and provenance blockers are recorded;
- the clean baseline can be reproduced without relying on historical local
  copies or transient development workspaces.

This stage is not product feature work. It protects the validity of all later proofs.

---

## 1. Canonical automation-coherence rule pack

The first product slice is a bounded automation audit, not a universal compliance scanner.

Current target:

- one canonical `automation-coherence` rule pack;
- versioned deterministic controls;
- explicit evidence requirements;
- stable outcomes for detected finding, no finding detected and not evaluable;
- synthetic fixtures for anomalous, healthy and missing-evidence cases;
- no claim that the absence of a finding proves overall conformity;
- no agent authority over deterministic or human decisions.

The initial controls focus on:

- duplicate execution of the same business consequence;
- execution incompatible with a recorded business state;
- missing traceability or expected human validation for a sensitive action.

Exit criteria:

- the canonical rule pack and its digest are unambiguous;
- deterministic fixture results are reproducible;
- missing evidence produces an explicit bounded state;
- rule, evidence and finding identifiers remain linked through the full chain.

---

## 2. Strengthen portal end-to-end proof

The portal is not currently available. Construction and complete product
validation must be performed internally with non-sensitive fixtures before any
public availability or production-readiness claim.

Required journey:

1. sign in through the browser;
2. create a bounded audit;
3. provide or select authorized fixture sources;
4. freeze one evidence snapshot;
5. run deterministic controls and role-based analysis;
6. display findings, evidence and limitations;
7. obtain a human decision bound to the displayed review state;
8. generate and reload a stable report;
9. preserve sufficient proof artifacts to reproduce the run.

The test must also cover:

- retry and double-click without duplicate runs;
- partial source coverage;
- agent or evaluator unavailability;
- service restart and resume;
- clear failure states rather than false success;
- separation between agent contribution, deterministic result and human authority.

Exit criteria:

- the journey passes without manual API substitution, mocks or hidden database repair;
- the final projection records the human decision and report state;
- the evidence package includes versions, logs, projections and user-interface captures;
- an explicit Human GO authorizes movement to controlled external use.

---

## 3. Controlled portal validation before availability

The portal remains unavailable while construction and the internal end-to-end
proof are completed. A controlled validation stage follows before any broader
availability claim.

Initial perimeter:

- French-first user experience;
- one automation-coherence audit;
- controlled n8n-style workflow and execution input;
- one bounded business source such as a CRM export;
- read-only operation;
- explicit scope, time window and source limitations;
- client-side validation of findings;
- exportable report and evidence register.

Once opened, the portal should not require a manually accompanied audit for
every user. Human assistance may remain optional for qualification,
interpretation or a broader mandate. The separate Professional DUBSAR Audit is
available on request for organizations that want that human-led engagement.

Exit criteria:

- invited users can complete the journey without operator repair;
- support load, false positives and not-evaluable cases are understood;
- data handling, retention and deletion are documented;
- access remains controlled until reliability and security gates are met.

---

## 4. Bounded external validation

External validation begins with a small, explicitly authorized perimeter. It is not a production-wide customer deployment.

The first external users should validate:

- whether the audit captures useful evidence before interviews;
- whether findings are understandable and correctly bounded;
- whether human classification is practical;
- whether the report shortens discovery and prioritization work;
- which connector or context gaps still require interviews;
- whether the audit identifies a justified continuous-governance use case.

No claim should imply that interviews are always eliminated. The objective is to reduce avoidable discovery work and make remaining questions more targeted.

Exit criteria:

- users obtain a useful result without unsafe access or overclaiming;
- material failure and limitation cases are documented;
- the product value is demonstrated before expanding connector scope;
- any move to continuous governance is based on an audited need.

---

## 5. DUBSAR Node and continuous governance

Continuous governance follows the audit; it does not precede it.

DUBSAR Node is a separate scoped deployment path and is not generally
available.

Planned work:

- define a stable Node-to-Backend contract;
- install the Node in or near the customer environment;
- add administrator-facing health and connector controls;
- evaluate sensitive actions before execution;
- support bounded policy results such as `ALLOW`, `DENY`, `REQUIRE_HUMAN_APPROVAL` and conditional allow;
- keep protected credentials and actions outside agent prompts;
- preserve an attributable action and decision ledger;
- fail closed for protected actions when the authority path is unavailable.

Initial governed actions should be narrow and reversible where possible. Examples may include requiring approval before a sensitive outbound email or blocking an action that contradicts an explicit business state.

Exit criteria:

- one selected action is governed end to end in a controlled environment;
- the Node cannot bypass or impersonate the Core or Human Gate;
- retry, outage and recovery behavior are proven;
- administrators can understand system state and intervene safely.

---

## 6. Connector expansion

Connector breadth follows proof of the first audit, not the other way around.

Possible additions include:

- live n8n API or HTTP integration;
- CRM systems;
- email and messaging systems;
- Make and other automation platforms;
- code and project sources where relevant;
- generic event or evidence ingestion.

Each connector must define:

- minimum required permissions;
- fields collected and excluded;
- pagination, truncation and time-window behavior;
- version and change detection;
- explicit degraded and unavailable states;
- retry and idempotency behavior;
- test fixtures independent of the third-party service.

DUBSAR rules and canonical decisions must remain independent of any one connector vendor.

---

## 7. AI governance and AI Act preparation

Regulatory requirements may inform dedicated rule packs and report structures.

Possible product support includes:

- system and agent inventory;
- purpose, owner and responsibility records;
- traceability of evidence, versions, decisions and actions;
- documented human oversight;
- limitation and incident records;
- exportable governance evidence.

This work must remain within a clear boundary:

- no legal advice;
- no automatic legal verdict;
- no claim of certification;
- no conversion of incomplete evidence into compliance;
- dated and versioned regulatory mappings;
- review by appropriate legal or compliance professionals when required.

---

## 8. Coding-agent product and future adapters

DUBSAR for Claude Code is a parallel functional controlled private beta being
finalized. Access is selective and invitation-based, with Windows as the first
supported target. Codex and Cursor remain future adapter paths.

The earlier desktop, bridge and plugin work may contribute:

- local runtime and process control;
- workspace and session identity;
- decision continuity;
- evidence capture;
- Human Gate presentation;
- technical administrator experience.

These integrations should reuse the same private Core and authority model. They
must not become separate product brains or delay the portal-first audit.

The public Claude Code Marketplace is inactive. The controlled beta is not a
public Marketplace or general-availability claim, and no availability is
claimed for Codex or Cursor.

---

## Explicitly out of scope for the current claim

- a real agency pilot before internal browser end-to-end acceptance;
- general availability of the portal;
- production deployment of DUBSAR Node;
- broad live-connector coverage;
- autonomous approval or self-certification by an agent;
- guaranteed replacement of discovery interviews;
- AI Act certification or legal compliance verdicts;
- public distribution of the private Core;
- general availability of DUBSAR for Claude Code;
- public Claude Code Marketplace distribution;
- supported Codex or Cursor products.

---

## Current status

```text
foundation reconciliation: in progress
first deterministic rule pack: internal validation
full portal browser E2E: not yet proven
automated audit portal: coming soon, under construction and validation, not available
professional DUBSAR Audit: available on request
DUBSAR for Claude Code: functional controlled private beta being finalized
coding-agent beta access: selective invitation, Windows first
public Claude Code Marketplace: inactive
DUBSAR Node: separate scoped deployment path, not generally available
Codex and Cursor adapters: future
bounded external portal validation: next stage
private Core: proprietary, not distributed
general production availability: not claimed
```
