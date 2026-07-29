# DUBSAR Audit

DUBSAR Audit is the portal-first entry point to DUBSAR.

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

The complete browser-based journey has **not yet been proved end to end as a
normal user**. In particular, the current evidence does not establish a
generally available self-service portal from sign-in through upload, review,
reload and report export.

Until that proof exists:

- the portal remains under internal, access-controlled validation;
- API-level evidence must not be described as a user-interface E2E;
- a zero-finding result means “no finding detected in the bounded scope,” not
  “the automation is compliant”;
- an unavailable or incomplete source remains visible and may make a control
  not evaluable.

See [Current status](STATUS.md) for the latest product boundary.

## What the report is intended to contain

When the portal journey is validated, the report is intended to contain:

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

The audit is intended to lead to continuous governance when a customer chooses
to go further.

A future installed **DUBSAR Node**, administered through the desktop, is
intended to connect selected automation and agent execution paths to the private
DUBSAR Core. Depending on the system, that boundary may use a controlled HTTP
gateway, API or host adapter. It may prepare sensitive actions for human
approval and later enforce bounded policy decisions.

That installed governance path is future product work. It is not currently
presented as a production-ready deployment.

Claude Code, Codex, Cursor and other developer-host adapters remain a secondary
Developer Labs direction. They are not prerequisites for the portal audit and
are not claimed as generally available integrations.

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

## Optional professional support

The product target is a self-service audit through the portal, without requiring
Sofiane to review every initial run.

An optional guided engagement may be offered later for scoping, interpretation,
remediation planning or installation. It is a separate service and must not be
presented as mandatory portal operation or as currently available until it is
explicitly announced.

## Follow the validation

The public method is described at [dubsar.ai/audit](https://dubsar.ai/audit).
Portal access will be presented as available only after its access controls and
complete user journey have been validated.
