# FAQ

## What is DUBSAR?

DUBSAR is a governance system for AI automations and agents.

It is designed to connect actions to evidence, expose contradictions and
missing information, keep deterministic controls separate from model
explanations, and preserve explicit human authority over sensitive decisions.

The current product direction starts with an automation audit in the portal,
then extends toward continuous governance and orchestration through an installed
DUBSAR Node.

---

## Is DUBSAR another AI or coding agent?

No. DUBSAR is not another general-purpose model and does not replace the tools
that perform the work.

It can coordinate specialized agent roles, but an agent does not govern itself.
The private DUBSAR Core owns canonical state and deterministic policy; agents
may analyze, explain and propose; humans retain protected decisions.

---

## What problem does DUBSAR address first?

Automation behavior is often spread across workflow tools, CRM records,
messages, business state and human approvals. A single system may show that an
action ran without establishing whether it was duplicated, compatible with the
current business state or properly validated.

DUBSAR begins by freezing a bounded evidence scope and testing specific
cross-system coherence questions without inventing causality.

---

## What is the first product surface?

The first product surface is the DUBSAR audit portal.

Its initial target journey is:

1. provide explicitly authorized, bounded sources;
2. freeze the evidence snapshot and coverage;
3. run deterministic controls;
4. display every candidate finding with its evidence and limitations;
5. let a human mark it true, false or uncertain;
6. generate an evidence-linked report.

This is the target journey. It is not yet a claim of general availability.

---

## What is the first Rule Pack?

The first Rule Pack is **automation coherence**. Its initial working profile
uses bounded n8n and HubSpot exports to look for:

- duplicate consequences without an attributable idempotency boundary;
- actions incompatible with the available business state;
- missing traceability or expected human validation for a sensitive action.

A missing record is reported as “no proof found in the connected sources.” It
is not turned into a claim that the record or event never existed.

---

## Must a customer use n8n and HubSpot?

They are the first bounded evidence profile, not the permanent product limit.

Other systems will require explicit source contracts, normalization,
completeness semantics and test fixtures before support is claimed. A logo or a
generic connector is not enough to establish a reliable audit.

---

## Does DUBSAR prove causality?

No.

DUBSAR can establish bounded observations and deterministic relationships in
the evidence it received. It must keep observed, derived, inferred,
not-captured and unavailable information distinct.

Temporal proximity or a plausible model explanation does not become proof of
causality.

---

## Is the audit fully automated?

The target workflow automates collection, normalization, deterministic checks
and report preparation where the evidence contract allows it.

It does not automate away responsibility:

- deterministic evaluators produce bounded results;
- agents may explain and structure candidate findings;
- a human reviews each proposed finding;
- incomplete evidence remains incomplete;
- no agent-generated statement becomes final by itself.

---

## What is a Human Gate?

A Human Gate is an explicit, attributable decision at a protected point in the
workflow.

For the first portal audit, the human reviews the evidence shown for a candidate
finding and records a disposition such as true, false or uncertain. A model
cannot create that decision by claiming that approval occurred.

Future continuous-governance paths may also use Human Gates before a sensitive
business action is released.

---

## What is currently proved?

The automation-coherence evaluator has been exercised on synthetic fixtures. A
controlled deployment also recorded an API-level audit path.

That does **not** yet prove the complete portal journey as a normal user. The
browser flow from sign-in and source upload through review, reload and report
export still requires a full user-interface E2E proof.

A reachable page, successful account creation or working API route is not, by
itself, proof that the product journey works.

See [Current status](STATUS.md).

---

## Is the portal publicly available?

Not as a generally available, production-ready product.

The portal remains under internal, access-controlled validation until its
security boundary and complete user journey are proved. Public documentation
must not turn a reachable deployment or an API test into an availability claim.

---

## What does a zero-finding result mean?

It means that no candidate finding was detected by the selected controls in the
bounded evidence scope.

It does not mean that the automation is complete, defect-free, secure or
compliant. A missing source may make a control not evaluable rather than
successful.

---

## What happens after the audit?

The intended next step is continuous governance when a customer chooses to
instrument selected automation or agent paths.

A future installed **DUBSAR Node**, administered through the desktop, is
intended to connect those paths to the private Core through a controlled HTTP
gateway, API or host adapter. It may prepare sensitive actions for human
approval and later apply bounded policy decisions.

This is future product work, not a production-ready deployment claim.

---

## What is the difference between the portal, Node and desktop?

- **Portal:** the user-facing audit journey, evidence review and reports.
- **DUBSAR Node:** the future installed boundary between selected customer
  systems and DUBSAR governance.
- **Desktop:** the future administrative cockpit for technical operators to
  configure, observe and maintain that installed boundary.
- **Private Core:** the canonical authority for governed state, evidence
  relationships, policy and Human Gates.

They are product surfaces with different responsibilities, not separate
governance brains.

---

## Does DUBSAR replace n8n, Make or other automation tools?

Replacement is not the first product claim.

The first audit is designed to work from bounded evidence produced by existing
systems. Future governance and orchestration may coordinate DUBSAR-managed
agents or sit on selected action paths, but support must be proved integration
by integration.

DUBSAR should not depend on undocumented behavior or pretend that a connector
removes the need for a stable contract.

---

## Where do Claude Code, Codex and Cursor fit?

Developer-host adapters are a secondary Developer Labs direction.

They explore how the same Core principles—canonical state, evidence, explicit
authority and replay—can govern agent-assisted development. They are not
prerequisites for the portal audit and are not the primary commercial entry
point.

No generally available Claude Code, Codex or Cursor integration is claimed
today.

---

## Is the Claude Code Marketplace live?

No.

This repository may contain historical or staging Marketplace material. It is
not a supported public installation path, and no visible command or source tree
should be treated as an active release until publication is explicitly
authorized.

---

## Which operating systems are supported?

There is no generally available Node or desktop distribution today.

Historical Windows engineering work established packaging and installation
building blocks, but it did not prove the current portal-to-Node product
journey. Linux and macOS support must not be claimed before their real package,
permissions, storage, update and removal paths are validated.

---

## Does DUBSAR certify AI Act compliance?

No.

DUBSAR is being designed to support evidence traceability, system inventory,
documented limitations and explicit human oversight. These capabilities may
help an organization prepare documentation and controls relevant to the EU AI
Act.

DUBSAR does not provide legal advice, determine legal applicability, assign an
authoritative risk classification or certify compliance. The provider,
deployer and relevant professional or public authorities retain their own
responsibilities.

---

## Is DUBSAR read-only?

The audit starts read-only by default: no ticket, message, correction or
external mutation is created merely because an audit ran.

Future continuous governance may deliberately mediate selected actions. Such a
path will require an explicit policy, narrow credentials, attributable Human
Gates, fail-closed behavior and separate validation. It must not be implied by
the current audit.

---

## What data does the public website collect?

The public marketing website must not request connector credentials, tokens or
source archives.

The portal has a different data boundary. Its authentication, source imports,
retention, deletion, logs, subprocessors and model-provider flows must be
documented and validated before general availability. See [Privacy](PRIVACY.md)
and [Security](SECURITY.md) for the published boundary.

---

## Is DUBSAR open source?

The whole DUBSAR product is not open source.

The private Core and private Backend implementation are not distributed here.
Public documentation, staging adapter material and third-party components are
governed by their respective licences and notices. Public visibility does not
create an open-source licence grant.

Distribution remains subject to component provenance, dependency and licence
review.

---

## What happened to the SCRIBE name?

DUBSAR is the public product.

Some historical repository, command, schema, MCP, environment or local-storage
identifiers may still contain `scribe` while compatibility work continues.
They are implementation identifiers, not a second current product and not an
availability claim.

---

## Is professional support required?

No. The product target is a self-service first audit through the portal.

An optional guided service may be offered later for scoping, interpretation,
remediation planning or installation. It is separate from normal portal
operation and must not be described as currently available until it is
explicitly announced.

---

## Is DUBSAR beta-ready or production-ready?

No generally available or production-ready product is claimed today.

The deterministic automation controls and parts of the API path have evidence.
The complete portal UI journey, installed Node, administrative desktop and
continuous-governance path still require their own end-to-end proofs.

“Implemented,” “API-tested,” “interface demonstrated,” “user E2E proved” and
“production-ready” are different statuses and must remain different.

---

## Where can I follow the project?

Start with [dubsar.ai](https://dubsar.ai/) and the
[DUBSAR audit method](AUDIT.md). Public access or support options will be
announced only when their corresponding product boundaries have been validated.
