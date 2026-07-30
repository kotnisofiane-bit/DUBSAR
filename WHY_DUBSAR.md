# Why DUBSAR?

DUBSAR began with a broader question than code generation:

> How can people remain in control when work is distributed across
> automations, AI agents, tools and sessions?

The first experiments focused on coding agents. They exposed a general problem
that also exists in business automation: actions can be fast and locally
reasonable while their origin, evidence and approval path become difficult to
reconstruct.

DUBSAR is now being developed as an evidence-first audit and governance layer
for business automations and AI agents.

[Back to the README](README.md) · [Version française](README.fr.md)

---

## Automation creates an evidence problem

A business action may depend on:

- a workflow version;
- data from one or more business systems;
- a prompt or agent instruction;
- a model response;
- a retry or idempotency mechanism;
- an approval rule;
- a human decision.

The tools executing those steps may each record part of the story. Few preserve
the whole decision path in one bounded, reviewable form.

As a result, an organization can know that an action happened without being
able to show precisely:

- why it happened;
- whether it was compatible with the known business state;
- whether the same event triggered it twice;
- which evidence was missing;
- whether a required human validation was actually captured.

This is the gap DUBSAR addresses first.

---

## Audit comes before orchestration

DUBSAR's intended first product path is not to replace n8n, an automation
platform or an agent runtime.

It is designed to begin with a portal audit because responsible governance
needs an initial picture of the existing system:

1. define an authorized scope;
2. collect bounded evidence;
3. freeze a reproducible snapshot;
4. apply deterministic controls;
5. use specialized agents only within explicit roles;
6. present proposed findings and their limitations;
7. require a human decision;
8. preserve a traceable report.

The automated portal implementing this journey is coming soon. It remains
under development and validation and is not currently available for public
use.

This first audit can later become the foundation for continuous governance:
policy evaluation, recurring evidence collection, controlled orchestration and
Human Gates before sensitive actions. Those capabilities remain roadmap items,
not current production claims.

---

## Why a deterministic Core?

An agent can inspect context, explain a contradiction and propose a course of
action. It should not be the sole authority deciding whether its own work is
valid.

The private DUBSAR Core is intended to preserve:

- canonical identities and state;
- evidence snapshots and digests;
- deterministic control execution;
- decision and review records;
- explicit Human Gates;
- the distinction between facts, inferences and unavailable evidence.

This provides a stable authority boundary around probabilistic systems.

**Model output is input to governance, not governance itself.**

---

## Why Hermes roles?

Hermes provides specialized agent roles within a bounded assignment. Depending
on the audit, a role may collect, inspect, explain, challenge or summarize
material.

Those roles are useful because an audit often requires several perspectives.
They remain non-authoritative:

- they cannot rewrite the frozen evidence;
- they cannot declare missing evidence verified;
- they cannot approve their own conclusions;
- they cannot bypass the deterministic Core or a Human Gate.

The value is not “more agents.” The value is role separation under a stable
control system.

---

## Why human review?

Automation evidence is often incomplete. Business meaning may depend on facts
that no connector can observe.

DUBSAR therefore treats findings as proposals until a human reviewer confirms,
corrects or rejects them. The review must keep the evidence, scope and decision
path linked.

This does not transfer every task back to a human. It reserves human authority
for interpretation and protected decisions while allowing deterministic checks
and bounded agents to do repeatable preparation work.

---

## Why build a portal first?

The planned portal is intended to give non-developer users a common place to:

- define the audit scope;
- provide authorized sources;
- inspect evidence and proposed findings;
- record decisions;
- retrieve a bounded report.

It separates the business audit experience from the technical administration
surface.

A future local Node or desktop may support installation, credentials, local
execution and continuous governance inside a customer environment. It is a
prototype and roadmap direction, not the first generally available product.

DUBSAR for coding agents is a distinct controlled private-beta surface, with
Claude Code first. Codex, Cursor and similar adapters remain future directions.
This surface is real, but it is separate from the planned portal and is not a
generally available public product.

---

## Why keep the Core private?

Public adapters, schemas and examples can remain inspectable and
interoperable. The deterministic authority model and proprietary decision
mechanisms need a consistent protected implementation.

The private Core owns canonical governance state. This public repository
documents the product boundary and may distribute thin integration components;
it does not publish the private engine.

Using open-source components such as Hermes does not imply that the complete
DUBSAR product is distributed under one open-source license.

---

## Regulatory relevance without a certification claim

Governance regulations, including the EU AI Act, increase the importance of
inventory, traceability, human oversight, evidence provenance and documented
decisions.

DUBSAR is designed to help structure technical evidence relevant to that work.
It does not certify regulatory compliance, perform a legal conformity
assessment, or replace legal and compliance professionals.

The distinction is important: software can help collect and preserve evidence;
it cannot make every legal conclusion automatically.

---

## What success would look like

DUBSAR succeeds if an organization can move from:

> “The automation ran, but we cannot fully explain why.”

to:

> “Here is the bounded evidence, the deterministic control that fired, the
> agent analysis, the human decision, and the limits of what was observed.”

That is the foundation for accountable automation and, later, controlled
orchestration.

---

## Current boundary

Today, the DUBSAR marketing website and public documentation are publicly
available. The automated audit portal is coming soon: it remains under
development and validation and is not currently available for public use.
Deterministic controls and an API-backed audit path have internal technical
evidence. The complete end-to-end portal journey, production connectors,
continuous policy enforcement and local administration Node still require
further implementation and end-user validation.

Professional DUBSAR Audit remains available on request. DUBSAR for coding
agents remains a controlled private beta. No generally available Node
deployment is currently claimed.

DUBSAR distinguishes a prototype interface, an API proof and a real user
journey. Public claims will follow the evidence.
