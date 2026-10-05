# Roadmap

DUBSAR is being integrated as a control plane for durable, governed agentic
work. This roadmap describes technical priorities, not promised dates,
public access or a release schedule. [STATUS.md](STATUS.md) defines what is
currently claimed.

## 1. One coherent Personal mission

Connect My Work, Agents / Hermes, Memory, Automation, Tool Layer / Connectors,
Operational Context / Evidence, Judgment, Trace Canvas and Human Gates around
one durable mission identity.

The integration must preserve state and decisions across sessions and agent
or provider changes. Views should agree on the mission's recorded state,
supporting evidence, unresolved work and required decisions.

## 2. Desktop and Trace Canvas integration

Make the durable work and its evidence usable in the Desktop experience.
Trace Canvas should project recorded events and decisions with their limits.

Validation should cover resumption, partial sources, rejected actions and
the effect of changes to the underlying mission state. A visible screen alone
does not establish a complete user journey.

## 3. Bounded local Judgment

Integrate the current local candidate, Qwen, behind AgentContext / Judgment
contracts. Preserve a closed cognitive-move vocabulary and deterministic
validation independent of provider choice.

Unsupported references, malformed output and proposals beyond authority must
remain explicit failures. No model may create permissions, freshness,
evidence or mission completion.

## 4. Provider, automation and connector breadth

Extend coverage through documented contracts and bounded access.
Each integration needs explicit permissions, source versions, coverage,
failure states and attribution of execution results.

A connector's existence does not establish reliable mission-wide support.

## 5. Control Plane runtime qualification

Qualify the real path from Human / Core decision through signed
authorization / Task Lease, admission, durable handoff, workload / sandbox,
mediated egress, Gateway / Broker and returned evidence.

The work must exercise rejected admission, replay, interruption, recovery,
credential separation, uncertain external outcomes and required Human Gates.
Component tests do not substitute for qualification of the combined path.

## 6. Public technical source and release decisions

Link real public components from this root when their source, scope and
limits are ready for review. No publication of `dubsar-contracts` or other
private repositories is announced.

Any future Personal release needs an actual artifact and validated
installation, update and removal, supported environments, licensing,
security, privacy and support boundaries. No public beta or general
availability is implied by these priorities.

Earlier portal-audit and Marketplace roadmaps are historical. Their rationale
and records remain indexed in [LEGACY.md](LEGACY.md).
