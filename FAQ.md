# FAQ

## What is DUBSAR?

DUBSAR is an audit and governance system for AI automations and agents.

It is designed to connect actions to evidence, expose contradictions and
missing information, keep deterministic controls separate from model
explanations, and preserve explicit human authority over sensitive decisions.

The current direction has two delivery surfaces: an automated audit portal,
which is coming soon and remains under construction and validation, and the
Professional DUBSAR Audit, available on request.

---

## Is DUBSAR another AI or coding agent?

No. DUBSAR is not another general-purpose model and does not replace the tools
that perform the work.

Agents may analyze, explain and propose within a bounded assignment. They do not
govern themselves or approve their own conclusions. Human authority remains
explicit for protected decisions.

---

## What problem does DUBSAR address first?

Automation behavior is often spread across workflow tools, CRM records,
messages, business state and human approvals. A system may show that an action
ran without establishing whether it was duplicated, compatible with the
current business state or properly validated.

DUBSAR begins by freezing a bounded evidence scope and testing specific
cross-system coherence questions without inventing causality.

---

## What are the current product surfaces?

There are two:

1. the planned self-service DUBSAR audit portal;
2. the Professional DUBSAR Audit, available on request under an agreed mandate.

The portal prepares a structured first result. The professional audit adds
operator analysis, agreed permissions, human review and a professional
deliverable.

The portal is coming soon and is not currently available. The professional
service is available now on request.

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

Other systems require explicit source contracts, normalization, completeness
semantics and test fixtures before support is claimed. A logo or generic
connector is not enough to establish a reliable audit.

---

## Does DUBSAR prove causality?

No. DUBSAR can establish bounded observations and deterministic relationships
in the evidence it received. Observed, derived, inferred, not-captured and
unavailable information must remain distinct.

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

For the planned first portal audit, a human reviews the evidence for a candidate
finding and records a disposition such as true, false or uncertain. A model
cannot create that decision by claiming that approval occurred.

---

## What is currently proved?

The automation-coherence evaluator has been exercised on synthetic fixtures. A
controlled deployment also recorded an API-level audit path.

That does **not** prove the complete portal journey as a normal user. The
browser flow from sign-in and source upload through review, reload and report
export still requires complete end-to-end proof.

A reachable page, successful account creation or working API route is not, by
itself, proof that the product journey works.

See [Current status](STATUS.md).

---

## Is the portal publicly available?

No. The [DUBSAR audit page](https://dubsar.ai/audit) is public, but the
self-service portal is coming soon and is not currently available.
Construction, complete browser-journey validation and security validation are
still in progress.

---

## What does a zero-finding result mean?

It means that no candidate finding was detected by the selected controls in the
bounded evidence scope.

It does not mean that the automation is complete, defect-free, secure or
compliant. A missing source may make a control not evaluable rather than
successful.

---

## What happens after the audit?

The first outcome is a bounded report with its evidence, limitations and human
review.

Continuous governance or an installed local component may later be considered
under a separate scope when the audit establishes a real need. Its architecture,
distribution, supported platforms and licensing are undecided and not promised.

---

## Does DUBSAR replace n8n, Make or other automation tools?

No replacement claim is made.

The first audit is designed to work from bounded evidence produced by existing
systems. Any future integration or governed action path must be proved
individually through a stable, documented contract.

---

## Where do Claude Code, Codex and Cursor fit?

Earlier DUBSAR experiments explored governance around coding agents, including
a Claude Code staging package. Those experiments informed the evidence and
human-authority doctrine now used by DUBSAR.

They are not current product surfaces. No active public or private beta,
supported plugin, runtime or host integration is offered, and no availability
claim is made for Claude Code, Codex or Cursor.

---

## Is the Claude Code Marketplace live?

No.

The historical Marketplace manifest and vendored plugin runtime have been
retired from the active repository tree. The remaining tombstone is a
non-executable provenance record, not a supported installation path.

---

## What is `dubsar-agent-skills`?

The separate
[dubsar-agent-skills](https://github.com/kotnisofiane-bit/dubsar-agent-skills)
repository publishes MIT-licensed doctrine and bounded local helpers for audit
and governance work.

It is not the DUBSAR product, Portal, private Core or runtime.
It grants no access to private services and does not make DUBSAR installable or
generally available. Its MIT licence applies only to that repository.

---

## Which operating systems are supported?

The planned portal has a browser and service boundary; supported browser and
service conditions will be announced with availability.

There is no generally available installed DUBSAR product today. No Windows,
Linux or macOS support claim is made for one.

The separate public skills may be used only according to their own repository
instructions and do not establish DUBSAR platform support.

---

## Does DUBSAR certify AI Act compliance?

No.

DUBSAR is being designed to support evidence traceability, system inventory,
documented limitations and explicit human oversight. These capabilities may
help an organization prepare documentation and controls relevant to the EU AI
Act.

DUBSAR does not provide legal advice, determine legal applicability, assign an
authoritative risk classification or certify compliance.

---

## Is DUBSAR read-only?

The audit starts read-only by default: no ticket, message, correction or
external mutation is created merely because an audit ran.

Any future path that mediates selected actions would require an explicit
policy, narrow credentials, attributable Human Gates, fail-closed behavior and
separate validation. It must not be implied by the current audit.

---

## What data does the public website collect?

The public marketing website must not request connector credentials, tokens or
source archives.

The planned portal has a different data boundary. Authentication, source
imports, retention, deletion, logs, subprocessors and model-provider flows must
be documented and validated before it becomes available. See
[Privacy](PRIVACY.md) and [Security](SECURITY.md).

---

## Is DUBSAR open source?

The complete DUBSAR product is not open source.

The private Core and other private implementation are not distributed here. No
public software licence is currently selected or granted by this repository
for unpublished DUBSAR components. Any architecture, distribution or licensing
decision will be made separately if a concrete publication is ever considered.

The separate public skills repository is MIT-licensed. That licence does not
extend to this documentation repository or to private DUBSAR components.

Original DUBSAR documentation and assets remain rights-reserved unless a file
expressly states otherwise. Third-party components remain governed by their own
licences and notices. See [Rights and Licensing Status](RIGHTS.md).

---

## What happened to the SCRIBE name?

DUBSAR is the public product.

Some historical repository or implementation identifiers may still contain
`scribe`. They are not a second current product and do not establish an
availability or installation claim.

---

## Is the Professional DUBSAR Audit available now?

Yes. The self-service portal is still under construction, while the
Professional DUBSAR Audit is available on request as a separate, human-led
engagement. Scope, authorized sources, permissions, retention, deliverables,
timing and price are agreed before work begins. Read-only collection remains
the default.

See the [audit boundary](AUDIT.md),
[request an audit](https://dubsar.ai/audit) or
[contact Sofiane Kotni](mailto:kotni.sofiane@dubsar.ai).

---

## Is DUBSAR beta-ready or production-ready?

Status depends on the surface:

- the automated audit portal is coming soon, under construction and validation,
  and not currently available;
- the Professional DUBSAR Audit is available on request;
- the public skills are a separate MIT-licensed companion resource;
- the earlier coding-agent package is paused and no active beta exists;
- continuous governance or installed components may be considered later, but
  their architecture, distribution, support and licensing are undecided.

No blanket production-readiness claim is made.

“Implemented,” “API-tested,” “interface demonstrated,” “user E2E proved” and
“production-ready” are different statuses and must remain different.

---

## Where can I follow the project?

Start with [dubsar.ai](https://dubsar.ai/), the
[DUBSAR audit page](https://dubsar.ai/audit), the
[DUBSAR audit method](AUDIT.md), the
[current status](STATUS.md) and the separate
[public skills repository](https://github.com/kotnisofiane-bit/dubsar-agent-skills).
