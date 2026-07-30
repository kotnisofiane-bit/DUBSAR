# Product and Surfaces

DUBSAR is one audit and governance system with two current delivery surfaces:

1. **Automated audit** through the DUBSAR portal;
2. **Professional DUBSAR Audit** operated under an agreed mandate.

They share one doctrine but are not the same offer and do not have the same
maturity.

---

## Product definition

DUBSAR helps organizations understand and govern automations and AI-assisted
systems. It connects authorized facts, decisions and evidence while preserving:

- provenance and versions;
- limitations and unavailable sources;
- uncertainty and contradictions;
- explicit human authority.

The shared operating principle is:

```text
Systems analyze and apply declared rules
DUBSAR preserves, relates and checks
Humans authorize and decide
```

DUBSAR does not grant an agent or technical component authority to approve its
own work.

---

## Shared doctrine

Both current surfaces follow the same boundaries:

- only authorized sources are examined;
- persuasive wording is not treated as proof;
- facts and inferences remain separate;
- evidence remains tied to its source and version;
- contradictions remain visible;
- missing sources become explicit limitations;
- read-only access is the default;
- protected movement requires explicit authorization;
- no agent conclusion becomes final without the required human review.

---

## Surface 1 — Automated audit portal

The DUBSAR portal is the planned self-service surface for a bounded automated
audit. It is under construction and validation and is not yet publicly
available. The current public entry point is the
[audit overview](https://dubsar.ai/audit).

Its intended responsibilities are to:

- collect the perimeter selected by the user;
- identify the period and authorized sources;
- connect available events and evidence;
- apply declared consistency checks;
- surface potential inconsistencies;
- distinguish unavailable information from negative findings;
- collect human classification;
- prepare a reviewable report.

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

The intended portal is designed to display evidence, show relationships,
prepare findings, record classifications and generate a report.

It is not intended to:

- turn an inference into a fact;
- silently consider an unavailable source compliant;
- issue a legal compliance verdict;
- authorize protected client actions by itself;
- remove the responsibility of the designated human owner.

The complete browser journey and its security and data boundaries remain under
construction and validation.

[Explore the automated audit](https://dubsar.ai/audit)

---

## Surface 2 — Professional DUBSAR Audit

Professional DUBSAR Audit is a bounded service operated by Sofiane with DUBSAR.
It is not simply the automated portal with a different label.

The professional surface adds:

- an agreed mandate;
- explicit permissions and source authorization;
- bounded collection;
- operator analysis;
- evidence and contradiction records;
- human classification and review;
- a professional report and evidence register;
- agreed retention, timing and price.

### Launch readiness

**Question:** Is the product genuinely ready to open to users?

The review may cover critical user journeys, installation, permissions, error
behavior, documentation, billing, data handling, tests and known limitations.
The conclusion may be GO, GO under conditions or NO-GO within the agreed scope.

### Agent governance

**Question:** Can the team explain and verify how the project was built and
approved?

The review may cover project intent, decisions, evidence, contradictions, agent
actions, human validations and the boundary between proposals and approved
movement.

```text
Agreed mandate and permissions
    ↓
Authorized project sources
    ↓
Bounded collection and analysis
    ↓
Evidence, contradictions and limitations
    ↓
Human review and classification
    ↓
Professional report and evidence register
```

Conclusions remain limited by the sources that exist and were authorized.

[Professional audit method](AUDIT.md)

---

## What is not a product surface

### Public skills

The separate
[dubsar-agent-skills](https://github.com/kotnisofiane-bit/dubsar-agent-skills)
repository contains MIT-licensed public doctrine and bounded local helpers for
audit and governance work.

It is a companion resource, not a DUBSAR product surface. It does not contain
the Portal, private Core, runtime or private product implementation; it grants no
access to private services and is not a supported DUBSAR installation. Its MIT
licence applies only to that repository.

### Earlier coding-agent experiments

Earlier experiments explored governance around coding-agent projects and a
Claude Code staging package. They informed DUBSAR's evidence and authority
model, but are not a current commercial surface, active beta or supported
integration.

No public plugin, runtime, Marketplace package or beta-access path is currently
offered. The historical staging record is retained only for provenance.

### Possible future continuous governance

Continuous governance or installed components may be considered later under a
separate scope. They are not included with a portal report or professional
audit. Their architecture, distribution, support and licensing are undecided
and are not promised.

---

## Public architecture boundary

The public product model separates evidence preparation from protected
authority:

| Layer | Public responsibility | Authority boundary |
|---|---|---|
| Portal or audit interface | Configure scope, display evidence, collect review and present reports | Cannot authorize protected actions alone |
| Analysis | Relate facts and surface candidate findings | Cannot convert inference into fact |
| Private implementation boundary | Preserve governed state and the declared authority model | Internal topology is not published or implied here |
| Human authority | Validate findings and authorize protected movement | Remains accountable for the decision |

This public description intentionally omits private implementation, internal
policies, credentials and deployment topology.

---

## AI Act boundary

DUBSAR can help structure documentation relevant to AI Act readiness,
including:

- system and agent inventories;
- purposes and designated owners;
- source and version traceability;
- human-oversight records;
- evidence registers;
- known limitations;
- uncertainty and missing information.

DUBSAR does not provide legal advice, certify regulatory compliance, produce an
automatic conformity verdict or replace a qualified assessment.

---

## Public and private boundary

This repository may publish:

- public doctrine and product documentation;
- bounded examples and diagrams;
- public security, privacy and integrity information;
- non-executable historical records.

It does not publish:

- the Portal or other private product implementation;
- the proprietary DUBSAR Core;
- private Backend implementation details;
- any current installable DUBSAR component;
- internal policies, prompts or sealed journals;
- confidential client or tester data;
- secrets, tokens or trust material.

No public software licence is currently selected or granted by this repository.
See [Rights and Licensing Status](RIGHTS.md).

---

## Current maturity summary

| Surface or resource | Maturity |
|---|---|
| Automated audit portal | Under construction and validation; coming soon, not publicly available |
| Professional DUBSAR Audit | Available on request |
| Public skills | Separate MIT-licensed companion resource |
| Historical coding-agent package | Paused; active Marketplace surface retired; no public package |
| Continuous governance / installed components | Possible later; architecture, distribution, support and licensing undecided |
| Private Core | Active, proprietary and protected |

The portal is intended to prepare a bounded first result. The professional
audit adds a mandate, operator analysis and human review. Human authority
remains final.
