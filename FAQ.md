# FAQ

## What is DUBSAR?

A governance foundation in development, primarily for integrators and teams
deploying AI agents for clients. It aims to connect durable mission state,
explicit authorisations, human decisions and execution evidence so teams can
hand over and resume work, including when outcomes remain uncertain.
State, evidence, bounded Judgment and authority remain distinct from the agent.
[README.md](README.md) is the canonical public entry point.

## How do Personal and Control Plane differ?

Personal is the first product expression: a Desktop experience for durable
missions. Control Plane applies the same responsibility model to heavier or
organisational workloads, with explicit authorisation, admission, handoff,
sandbox and mediated provider access.

The B2B priority retains Personal and the published technical sequence.
Both remain in technical development and integration. Full B2B validation
is underway; pilots are not currently open.
[Product surfaces](PRODUCT_SURFACES.md) explains their boundaries.

## Can I install Personal today?

No public installable Personal release or public beta is announced.
This repository contains documentation, not application code.
See [Installation](INSTALLATION.md).

## Where is the technical code?

[Technical components](README.md#technical-components) links available public
source. [DUBSAR Contracts — reference](https://github.com/kotnisofiane-bit/dubsar-contracts-reference)
is the public contracts-and-conformance repository: versioned schemas,
deterministic validators, selected reference implementations and synthetic
tests. It is not the private canonical `dubsar-contracts` development source,
the full Control Plane runtime or the unified Personal product. Other
repositories will be linked when their public source and scope are available.

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

## Does a request acknowledgement prove that an action happened?

No. For example, an ERP may acknowledge an order-creation request without
confirming that the order exists. This is illustrative, not an available
DUBSAR connector. The team must check the outcome before deciding whether to
retry, retaining the uncertainty and the next decision for whoever resumes
the mission. Receipt, the action's observed result and mission completion
remain distinct.

## What happened to the audit, Marketplace and Scribe surfaces?

They are earlier product phases, preserved in [LEGACY.md](LEGACY.md).
The audit is not the current offer. Earlier availability statements and
conceptual diagrams do not define current Personal or Control Plane support.

## Does DUBSAR certify compliance?

No. Evidence and human-oversight records can support review, but do not
produce automatic legal certification or complete source coverage.

## What licence applies?

[RIGHTS.md](RIGHTS.md) defines this repository's rights. Public component
repositories define their own licences; those licences do not extend to the
private Core or automatically apply to this documentation.
