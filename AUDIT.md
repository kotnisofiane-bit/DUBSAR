# DUBSAR Audit

The automated DUBSAR Audit portal is coming soon. It is under construction and
validation and is not currently available. It is distinct from the Professional
DUBSAR Audit, available on request as a bounded human-led engagement.

Its first target is a bounded **automation-coherence audit**: connect or import
authorized evidence from an automation system and a business system, detect
specific inconsistencies, let a human review every proposed finding, and produce
an evidence-linked report.

It is not a legal certification, a generic AI verdict or a claim that every
business process can be reconstructed automatically.

## First audit profile: automation coherence

The initial working profile uses bounded n8n and HubSpot exports. It asks three
questions:

1. Was the same business consequence executed more than once without an
   attributable idempotency boundary?
2. Was an action executed while the available business state indicated that it
   should not be?
3. Can the connected sources establish the workflow version, active rule and
   expected human validation for a sensitive action?

The third control is deliberately bounded. When the evidence is absent, DUBSAR
must say **“no proof found in the connected sources”**, not that the event or
validation never existed.

These controls produce candidate findings within a declared evidence scope.
They do not prove causality, completeness or regulatory compliance.

## Target self-service journey

The intended portal journey is:

```text
Create or open an audit space
    ↓
Authorize and provide bounded sources
    ↓
Freeze the evidence snapshot and coverage
    ↓
Run deterministic controls
    ↓
Explain candidate findings with agent assistance
    ↓
Human review: true, false or uncertain
    ↓
Generate the evidence-linked report
```

The human review is part of the product, not an exception path. A model may
explain, summarize or propose a classification, but it cannot promote its own
output to verified truth or create a Human GO.

## Current validation boundary

The automation-coherence evaluator has been exercised against synthetic
fixtures, and an API-level audit path has been recorded in a controlled
deployment.

The complete browser-based journey has **not yet been proved end to end to a
general-availability or production-readiness standard**. In particular, the
current evidence does not establish every path from sign-in through upload,
review, reload and report export under all supported operating conditions.

During construction and active validation:

- the portal remains unavailable to the public;
- API-level evidence must not be described as a user-interface E2E;
- a zero-finding result means “no finding detected in the bounded scope,” not
  “the automation is compliant”;
- an unavailable or incomplete source remains visible and may make a control
  not evaluable.

The public marketing website describes the intended audit method; it does not
provide access to the portal.

See [Current status](STATUS.md) for the latest product boundary.

## What the report is intended to contain

The report is intended to contain:

- the audit question, mandate and bounded scope;
- source records, versions, digests and coverage limitations;
- candidate findings tied to evidence references;
- observed facts separated from derived or inferred statements;
- uncertainty, missing evidence and unavailable sources;
- the human disposition of each proposed finding;
- prioritized follow-up actions;
- a reproducible report identifier and evidence register.

No report should imply that connected sources were complete unless their
coverage was actually established.

## Safety and authority boundaries

- Read-only collection is the default for an audit.
- The public marketing website does not request connector credentials, tokens
  or source archives.
- Source access must be explicit, bounded and attributable.
- No ticket, remediation, message or external mutation is created by default.
- An unavailable source is reported as a limitation, never silently treated as
  conformant or non-conformant.
- Deterministic control results, agent explanations and human decisions remain
  distinct records.
- The customer remains responsible for business and remediation decisions.

Portal data flows, retention, deletion, subprocessors and authentication must
be documented and validated before general availability.

## After the audit

The first outcome is a bounded report with its evidence, limitations and human
review.

Continuous governance or installed components may be considered later under a
separate scope when an audit establishes a real need. No architecture,
distribution model, supported platform, service boundary or licensing decision
has been selected or promised for that possible direction.

Earlier coding-agent experiments are not a current product surface or active
beta. The historical Claude Code Marketplace staging surface has been retired
from the active tree; no public package or supported integration is available.

## AI Act preparation boundary

DUBSAR is being designed to support practical governance work such as system
inventory, evidence traceability, documented limitations and explicit human
oversight. Those capabilities may help an organization prepare documentation
and controls relevant to the EU AI Act.

DUBSAR does not:

- determine by itself whether the AI Act applies to an organization or system;
- assign a legally authoritative risk classification;
- provide legal advice;
- certify compliance;
- replace the provider, deployer, legal counsel or competent authority.

## Professional DUBSAR Audit

The planned self-service portal is intended not to require Sofiane to review
every initial run. While it is under construction, the Professional DUBSAR
Audit remains available on request for organizations that need a guided mandate.

It is a separate, human-led engagement for agreed work such as scoping,
evidence review, interpretation, remediation planning or preparation of a
separately scoped installation. Scope, authorized sources, permissions,
retention, deliverables, timing and price are agreed before work starts.
Read-only collection remains the default, and the service does not provide
legal certification.

Requests can start through the
[professional audit page](https://dubsar.ai/audit) or
[contact@dubsar.ai](mailto:contact@dubsar.ai).

## Follow the validation

The portal is coming soon and remains unavailable while construction and
validation continue. The public method and professional engagement are
described at [dubsar.ai/audit](https://dubsar.ai/audit). Public doctrine and
bounded local helpers are available separately in the MIT-licensed
[dubsar-agent-skills](https://github.com/kotnisofiane-bit/dubsar-agent-skills)
repository; they are not the DUBSAR product or runtime.
