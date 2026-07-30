# Roadmap

This roadmap describes the current product direction. It is not a delivery
guarantee.

DUBSAR is a **portal-first audit and governance product for AI agents and
business automations** with two current delivery surfaces:

- the automated audit portal, coming soon and currently under construction and
  validation;
- the Professional DUBSAR Audit, available on request.

The sequence is deliberate:

```text
reconcile the foundation
  -> validate the first rule pack
  -> prove the portal journey end to end
  -> validate it with bounded external use
  -> expand evidence sources
  -> decide whether any later governance scope is justified
```

Earlier coding-agent packaging is paused and is not part of the current
commercial roadmap claim.

---

## 0. Reconcile the foundation

Current priority:

- identify the authoritative version of each active component;
- remove duplicate, stale and accidental artifacts from release paths;
- audit dependencies, licences and provenance before redistribution;
- document the public/private boundary;
- keep the private Core and confidential proof material outside the public
  repository;
- keep current public claims aligned across the site and repositories.

Exit criteria:

- every active component has one identified canonical source;
- retained changes are attributable and reviewable;
- licence and provenance questions are recorded without forcing premature
  component-licence decisions;
- public documentation does not expose or imply a private implementation.

---

## 1. Canonical automation-coherence rule pack

The first product slice is a bounded automation audit, not a universal
compliance scanner.

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

- rule and evidence identities remain linked through the result;
- deterministic fixture results are reproducible;
- missing evidence produces an explicit bounded state.

---

## 2. Prove the portal journey end to end

The portal is not currently available. Construction and complete product
validation must be performed internally with non-sensitive fixtures before any
public availability or production-readiness claim.

Required journey:

1. sign in through the browser;
2. create a bounded audit;
3. provide or select authorized fixture sources;
4. freeze one evidence snapshot;
5. run declared controls and bounded analysis;
6. display findings, evidence and limitations;
7. obtain a human decision bound to the displayed review state;
8. generate and reload a stable report;
9. preserve enough evidence to reproduce the run.

Validation must also cover retry behavior, partial coverage, unavailable
components, service restart, explicit failures and the separation of agent
contribution, deterministic result and human authority.

Exit criteria:

- the browser journey passes without manual API substitution or hidden repair;
- the final report preserves the human decision and evidence boundary;
- an explicit approval authorizes movement to bounded external use.

---

## 3. Controlled portal validation

A controlled validation stage follows internal end-to-end proof before any
broader availability claim.

Initial perimeter:

- French-first user experience;
- one automation-coherence audit;
- controlled workflow and execution input;
- one bounded business source such as a CRM export;
- read-only operation;
- explicit scope, time window and source limitations;
- user review of findings;
- exportable report and evidence register.

The separate Professional DUBSAR Audit remains available for organizations that
want a human-led mandate.

Exit criteria:

- invited users can complete the journey without operator repair;
- support load, false positives and not-evaluable cases are understood;
- data handling, retention and deletion are documented;
- access remains controlled until reliability and security gates are met.

---

## 4. Bounded external validation

External validation begins with a small, explicitly authorized perimeter. It is
not a production-wide customer deployment.

The first external users should validate:

- whether the audit captures useful evidence before interviews;
- whether findings are understandable and correctly bounded;
- whether human classification is practical;
- whether the report shortens discovery and prioritization work;
- which context gaps still require interviews;
- whether a later governance need is justified.

Exit criteria:

- users obtain a useful result without unsafe access or overclaiming;
- material failure and limitation cases are documented;
- value is demonstrated before expanding connector scope.

---

## 5. Evidence-source expansion

Connector breadth follows proof of the first audit.

Possible additions include:

- live n8n API or HTTP integration;
- CRM systems;
- email and messaging systems;
- Make and other automation platforms;
- code and project sources where relevant;
- generic event or evidence ingestion.

Each source contract must define minimum permissions, collected and excluded
fields, pagination, truncation, time windows, version detection, unavailable
states, retry behavior and test fixtures.

DUBSAR controls must remain independent of any one connector vendor.

---

## 6. AI governance and AI Act preparation

Regulatory requirements may inform dedicated rule packs and report structures.

Possible support includes:

- system and agent inventory;
- purpose, owner and responsibility records;
- traceability of evidence, versions, decisions and actions;
- documented human oversight;
- limitation and incident records;
- exportable governance evidence.

This work remains within a clear boundary:

- no legal advice;
- no automatic legal verdict;
- no claim of certification;
- no conversion of incomplete evidence into compliance;
- dated and versioned regulatory mappings;
- review by appropriate professionals when required.

---

## 7. Public doctrine and skills

The
[dubsar-agent-skills](https://github.com/kotnisofiane-bit/dubsar-agent-skills)
repository may continue to publish MIT-licensed doctrine and bounded local
helpers.

That work remains independently versioned and must preserve a clear boundary:

- the skills are not the DUBSAR product or a product-installation path;
- they contain no private Core, Portal, private implementation or runtime;
- they grant no access to private services;
- their MIT licence applies only to their own repository.

Public helpers may demonstrate the doctrine, but they do not prove portal
availability or production readiness.

---

## 8. Possible later governance scope

Continuous governance or installed local components may be considered after
the audit product establishes a justified need.

No architecture, local-versus-hosted boundary, distribution model, supported
platform, service contract, schedule or licence is selected or promised. Any
concrete proposal would require a separate product, security, privacy,
provenance, licensing and operational decision.

---

## Historical coding-agent work

Earlier DUBSAR experiments explored multi-session software-project governance
and a Claude Code Marketplace staging package. They provided useful technical
and doctrinal lessons.

That path is paused as a product direction:

- it is not a current commercial surface;
- no active public or private beta is offered;
- no Claude Code, Codex or Cursor support is claimed;
- the historical Marketplace surface is retired from the active tree;
- no future adapter or package publication is promised.

Any return to that direction would require a new product decision and current
evidence.

---

## Explicitly out of scope for the current claim

- general availability of the portal;
- broad live-connector coverage;
- autonomous approval or self-certification by an agent;
- guaranteed replacement of discovery interviews;
- AI Act certification or legal compliance verdicts;
- public distribution of the private Core;
- public installation of a DUBSAR local product;
- an active coding-agent beta or Marketplace package;
- supported Claude Code, Codex or Cursor integrations.

---

## Current status

```text
foundation reconciliation: in progress
first deterministic rule pack: internal validation
full portal browser E2E: not yet proved
automated audit portal: coming soon, under construction and validation
professional DUBSAR Audit: available on request
public skills: separate MIT-licensed companion resource
historical coding-agent package: paused; Marketplace surface retired
continuous governance / installed components: possible later; all implementation and distribution decisions undecided
private Core: proprietary, not distributed
general production availability: not claimed
```
