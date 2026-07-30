# Product and Surfaces

DUBSAR is one governance and audit system with three distinct product surfaces:

1. **Automated audit** through the DUBSAR portal;
2. **Professional DUBSAR Audit** operated under an agreed mandate;
3. **DUBSAR for coding agents**, currently a controlled private beta.

The surfaces share one doctrine and may share protected technical components.

They are not the same offer and must not be presented as having the same maturity.

---

## Product definition

DUBSAR helps organizations understand and govern automations and AI-assisted projects.

It connects authorized facts, decisions and evidence while preserving:

- provenance;
- versions;
- limitations;
- uncertainty;
- contradictions;
- explicit human authority.

The shared operating principle is:

```text
Systems analyze and apply declared rules
DUBSAR preserves, relates and checks
Humans authorize and decide
```

DUBSAR does not grant an agent or technical component the authority to approve its own work.

---

## Shared doctrine

Every DUBSAR surface follows the same boundaries:

- only authorized sources are examined;
- persuasive wording is not treated as proof;
- facts and inferences remain separate;
- evidence remains tied to its source and version;
- contradictions remain visible;
- missing sources become explicit limitations;
- read-only access is the default;
- protected movement requires explicit authorization;
- no agent conclusion becomes final without the required human review.

The same doctrine applies whether DUBSAR is examining an existing automation or governing a software project during construction.

---

## Surface 1 — Automated audit portal

The DUBSAR portal is the planned self-service surface for a bounded automated
audit. It is under construction and validation and is not yet publicly
available. The current public entry point is the
[audit overview](https://dubsar.ai/audit).

Its responsibilities are to:

- collect the perimeter selected by the user;
- identify the period and authorized sources;
- connect available events and evidence;
- apply declared consistency checks;
- surface potential inconsistencies;
- distinguish unavailable information from negative findings;
- collect human classification;
- prepare a reviewable report.

The intended journey is:

```text
Authorized sources
    ↓
DUBSAR Portal
    ↓
Cross-source analysis
    ↓
Potential findings and limitations
    ↓
Human classification
    ↓
Report
```

### Portal authority boundary

The portal can:

- display evidence;
- show relationships;
- prepare findings;
- record classifications;
- generate a report.

The portal cannot:

- turn an inference into a fact;
- silently consider an unavailable source compliant;
- issue a legal compliance verdict;
- authorize protected client actions by itself;
- remove the responsibility of the designated human owner.

### Portal maturity

The portal is under construction and active validation. It is coming soon and
is not currently presented as publicly accessible, generally available or
production proven.

[Explore the automated audit](https://dubsar.ai/audit)

---

## Surface 2 — Professional DUBSAR Audit

Professional DUBSAR Audit is a bounded service operated by Sofiane with DUBSAR.

It is not simply the automated portal with a different label.

The professional surface adds:

- an agreed mandate;
- explicit permissions;
- bounded collection from authorized sources;
- operator analysis;
- DUBSAR evidence and contradiction records;
- human classification and review;
- a professional report;
- an evidence register;
- agreed retention, timing and price.

The primary mandates are:

### Launch readiness

**Question:** Is the product genuinely ready to open to users?

The review may cover:

- critical user journeys;
- installation;
- permissions;
- error behavior;
- documentation;
- billing;
- data handling;
- tests;
- known limitations.

The result may be:

- GO;
- GO under conditions;
- NO-GO.

### Agent governance

**Question:** Can the team explain and verify how the project was built and approved?

The review may cover:

- Mission continuity;
- decisions;
- evidence;
- contradictions;
- agent actions;
- human validations;
- the boundary between generated proposals and approved movement.

### Professional audit journey

```text
Agreed mandate and permissions
    ↓
Authorized project sources
    ↓
Bounded collection and analysis
    ↓
DUBSAR evidence, contradiction and decision records
    ↓
Human review and classification
    ↓
Professional report and evidence register
```

The service may examine a project that was not already using the DUBSAR coding-agent product.

Its conclusions remain limited by the sources that exist and were authorized.

[Professional audit method](AUDIT.md)

---

## Surface 3 — DUBSAR for coding agents

DUBSAR for coding agents governs long-running, multi-session software projects assisted by AI coding agents.

It adds a persistent project layer around existing agents without rebuilding their native capabilities.

```text
Coding agents build
DUBSAR preserves Mission, decisions, boundaries and evidence
Humans decide protected movement
```

Claude Code is the first host.

Codex, Cursor and other adapters remain future direction and are not currently available integrations.

### 3.1 Host adapter

A host adapter connects a coding-agent environment to DUBSAR.

For Claude Code, the adapter is the DUBSAR plugin.

Its role is to:

- propagate the native host session identity;
- expose bounded DUBSAR commands and tools;
- recognize or resume governed workspace context;
- display bounded canonical project state;
- connect the host to the local DUBSAR runtime;
- surface the next action and Human Gate status.

The adapter remains thin.

It does not contain the proprietary Core and does not make canonical business decisions locally.

Some command, MCP and environment identifiers may retain a temporary `scribe` prefix for compatibility. Public labels use DUBSAR.

### 3.2 Local Bridge

The Bridge provides bounded local transport between the host adapter and the local runtime.

It may support:

- local continuity references;
- closed request and response transport;
- start and status orchestration;
- session-to-runtime connectivity.

The Bridge is not the source of truth for Mission, decisions, evidence or Human Gates.

### 3.3 DUBSAR Desktop and local runtime

DUBSAR Desktop supplies the local runtime required by the current Claude Code integration.

Its responsibilities include:

- bounded local process startup;
- process identity and lifecycle control;
- governed worktree provisioning;
- restart observations and reconciliation requests;
- secure local configuration;
- navigation to cockpit and Human Gate surfaces.

Desktop is not marketed as a separate product and is not the private Core.

The legacy term “Launcher” may remain internally where changing it would break compatibility. It is not a separate public brand.

### 3.4 Multi-session governance

DUBSAR relates several active sessions to one Mission while preserving isolation.

```text
Mission
  ├── Session A → Worktree A → Process A → Evidence A
  └── Session B → Worktree B → Process B → Evidence B
                 ↓
          Conflict or Human Gate when required
```

Internal Windows proofs have validated this model.

The complete external product journey remains under validation.

---

## Optional deployment path — continuous governance

Continuous governance may be proposed separately after an audit when the need is established.

A DUBSAR Node is intended to apply declared controls inside an authorized client environment.

Conceptually:

```text
Proposed action
    ↓
DUBSAR Node
    ↓
Declared rule evaluation
    ↓
Authorized action
or
Human Gate
```

A Node:

- operates only within an agreed perimeter;
- must not create its own permissions;
- must not silently expand its authority;
- must preserve the relationship between action, rule and authorization;
- must stop or request human review when protected authority is required.

The Node is not automatically included with a portal report or professional audit.

No generally available Node deployment is currently claimed.

---

## Protected technical components

The three product surfaces may rely on shared protected components.

### DUBSAR Portal

The Portal is designed to support:

- configuration;
- source selection;
- findings;
- evidence display;
- human classification;
- reporting;
- visibility into governed state.

The Portal makes state understandable. It is not the final authority over protected actions.

### Private Backend

The Backend is the protected service boundary.

Its responsibilities include:

- validating requests;
- limiting scope;
- verifying runtime bindings;
- rejecting stale or unauthorized mutations;
- protecting private implementation details.

The Backend is not distributed through this repository.

### Private DUBSAR Core

The Core owns canonical governed state, including:

- Mission;
- decisions and constraints;
- evidence relationships;
- contradictions;
- audit state;
- declared rules;
- Human Gates;
- authorizations;
- replay and reconciliation state.

The Core can evaluate declared rules and preserve canonical outcomes.

It cannot grant itself authority outside the agreed policy and authorization model.

Human authority remains explicit for protected movement.

### Runner

The Runner produces bounded mechanical evidence such as:

- snapshots;
- diffs;
- test results;
- hashes;
- execution artefact references.

The Runner does not own Mission state and cannot create a Human GO.

### Cockpit

The cockpit makes governed state readable to the human.

It may display:

- recognized projects;
- active Missions;
- sessions;
- contracts and worktrees;
- decisions and constraints;
- declared and verified evidence;
- conflicts;
- stale state;
- pending Human Gates;
- availability and diagnostic information.

The cockpit cannot approve its own state.

The former label “Eyes of SCRIBE” is historical and must not remain a separate public product brand.

---

## Authority model

DUBSAR separates analysis, rules, execution and authority.

| Layer | Role | Authority boundary |
|---|---|---|
| Portal | Configure, display, classify and report | Cannot authorize protected actions alone |
| Analysis components | Relate facts and surface findings | Cannot convert inference into fact |
| Core | Preserve canonical state and evaluate declared rules | Cannot expand its own authority |
| Node | Apply authorized controls | Cannot act outside its mandate |
| Runner | Produce mechanical evidence | Cannot approve movement |
| Agent | Propose or perform bounded work | Cannot approve its own work |
| Human authority | Validate findings and authorize protected movement | Remains accountable for the decision |

The intended doctrine is not “the Core replaces the human.”

It is:

**The Portal makes evidence visible. The Core preserves state and applies declared rules. The Node enforces authorized controls. Humans retain final authority.**

---

## AI Act boundary

DUBSAR can help structure documentation relevant to AI Act readiness, including:

- system and agent inventories;
- purposes and designated owners;
- source and version traceability;
- human-oversight records;
- evidence registers;
- known limitations;
- uncertainty and missing information.

DUBSAR does not:

- provide legal advice;
- certify regulatory compliance;
- produce an automatic conformity verdict;
- replace a qualified legal or conformity assessment.

---

## Public and private boundary

This repository is intended to remain:

- the public doctrine and documentation repository;
- the future distribution home for authorized thin host adapters;
- a bounded source of examples, diagrams and public trust information.

It may contain:

- public product doctrine;
- public architecture descriptions;
- bounded examples;
- security and privacy information;
- installation boundaries;
- authorized adapter metadata.

It does not publish:

- the proprietary DUBSAR Core;
- private Backend implementation details;
- internal policies or prompts;
- sealed journals;
- confidential client or tester data;
- secrets, tokens or trust material.

---

## Platform boundary

### Automated audit portal

Web-based surface under construction and validation. It is not currently
presented as publicly accessible; the marketing audit page remains public.

### Windows

First controlled private-beta target for the coding-agent product.

### Linux

Planned for later validation. Not currently announced.

### macOS

Not currently announced. Packaging, signing and runtime behavior remain to be evaluated.

### Claude Code

First coding-agent integration and current engineering focus.

### Codex, Cursor and other hosts

Future adapter direction. Not currently supported publicly.

---

## Current maturity summary

| Surface | Maturity |
|---|---|
| Automated audit portal | Under construction and validation; coming soon, not publicly available |
| Professional DUBSAR Audit | Available on request |
| DUBSAR for Claude Code | Functional controlled private beta |
| External coding-agent access | Selective, invitation only |
| Public Marketplace | Historical staging surface retired from the active tree; no public package |
| DUBSAR Node | Separate scoped path, not generally available |
| Codex / Cursor | Future direction |
| Private Core | Active, proprietary and protected |

---

## Summary

DUBSAR is one governance and audit system.

The automated portal is intended to prepare a bounded first result.

The professional audit adds a mandate, operator analysis and human review.

The coding-agent product governs software projects during construction.

The Portal is designed to make evidence readable. The Backend protects
requests. The Core preserves canonical state and evaluates declared rules. The
Runner produces mechanical evidence. The Node applies only authorized controls.
The cockpit surfaces governed state. Human authority remains final.
