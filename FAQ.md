# FAQ

## What is DUBSAR?

A control plane for durable, governed agentic work. It separates mission
state, evidence, bounded judgment and authority from the agent doing the work.
[README.md](README.md) is the canonical public entry point.

## How do Personal and Control Plane differ?

Personal is the first product expression: a Desktop experience for durable
missions. Control Plane applies the same responsibility model to heavier or
organizational workloads, with explicit authorization, admission, handoff,
sandbox and mediated provider access.

Both remain in technical development and integration.
[Product surfaces](PRODUCT_SURFACES.md) explains their boundaries.

## Can I install Personal today?

No public installable Personal release or public beta is announced.
This repository contains documentation, not application code.
See [Installation](INSTALLATION.md).

## Where is the technical code?

[Technical components](README.md#technical-components) links available public
source. DUBSAR Memory is a separate technical preview; it is not the unified
Personal product. Other repositories will be linked when public source and
scope are available. `dubsar-contracts` is not presented as public.

## What does Judgment do?

It proposes a next cognitive move from a closed set, such as `consult`,
`conclude`, `clarify`, `revise` or `stop`. Software validates the proposal
and permits execution only under the applicable authority.

Judgment cannot create permissions, evidence, freshness, completion or actual
execution success. Qwen is the current local candidate, not the architecture.

## What is a Human Gate?

An attributable human decision bound to the scope, state, evidence,
limitations and consequential effect under review. An agent cannot create
that decision by asserting that approval happened.

## Is the whole Control Plane integrated live?

That claim is not made. Component tests and E2E qualifications apply only
to the exercised paths. Complete real-world runtime qualification remains
work in progress. See [Status](STATUS.md).

## Does a successful execution complete a mission?

Only the operation's bounded result has been observed. Mission completion
requires support for the mission's acceptance conditions. Neither event
automatically establishes proof of all surrounding claims.

## What happened to the audit, Marketplace and Scribe surfaces?

They are earlier product phases, preserved in [LEGACY.md](LEGACY.md).
Their availability statements and conceptual diagrams do not define current
Personal or Control Plane support.

## Does DUBSAR certify compliance?

No. Evidence and human-oversight records can support review, but do not
produce automatic legal certification or complete source coverage.

## What licence applies?

[RIGHTS.md](RIGHTS.md) defines this repository's rights. Public component
repositories define their own licences; those licences do not extend to the
private Core or automatically apply to this documentation.
