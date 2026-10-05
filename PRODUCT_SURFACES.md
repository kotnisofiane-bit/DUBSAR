# Product and Surfaces

DUBSAR is a control plane for durable, governed agentic work. Personal and
Control Plane express one architecture in two environments.

| Environment | Purpose | Current boundary |
|---|---|---|
| DUBSAR Personal | A Desktop experience for durable individual missions | Active integration / technical development; no public installable release |
| DUBSAR Control Plane | Govern heavier or organizational agentic workloads | Component boundaries and qualification work; full live integration not claimed |

These are product and architecture directions, not two generally available
offers. [STATUS.md](STATUS.md) is authoritative for maturity.

## DUBSAR Personal

Personal is the first product expression. My Work anchors durable missions;
Agents / Hermes execute assignments; Memory preserves continuity; Automation
and Tool Layer / Connectors connect execution and sources.

Operational Context / Evidence supplies bounded observations and provenance.
Judgment proposes a next cognitive move. Trace Canvas is intended to show
the recorded work path and decisions. Human Gates keep consequential effects
under explicit authority.

The integration goal is one coherent mission across all these views.
Users should be able to change agents or model providers without losing
the work itself. A view is a projection, not a competing source of state.

Desktop, Trace Canvas, local Judgment and provider / connector breadth remain
active integration work. No supported public Personal installation, beta
access or commercial support is announced.

## DUBSAR Control Plane

Control Plane applies the common model to heavier workloads:

```text
Human / Core decision
→ Signed authorization / Task Lease
→ Runtime admission
→ Durable handoff
→ Workload / sandbox
→ Mediated egress
→ Gateway / Broker
→ Evidence / Operational Context
```

The design places canonical state and authority in deterministic software.
An agent does not own provider credentials, create permissions or approve
itself. Admission and replay decisions must be deterministic. Crash recovery
must not silently create a second execution.

The combined path still needs qualification in its real runtime boundaries.
A tested component does not establish a complete organizational platform.

## Shared Judgment boundary

Judgment is a bounded probabilistic policy/controller with a closed action
vocabulary. It proposes; software validates; policy and Human Gates remain
authoritative. Qwen is the current local candidate, not the identity of
DUBSAR.

[ARCHITECTURE.md](ARCHITECTURE.md#judgment-contract) defines the public
responsibility model and what Judgment cannot do.

## Public entry point and source

This repository is the canonical public documentation root. Available
technical source is listed under [Technical components](README.md#technical-components).
Component source, licences and tests apply to their own documented scope;
they do not imply availability of unified Personal or Control Plane.

The former automated audit portal, Professional DUBSAR Audit, Marketplace
staging and Scribe line are historical product phases indexed in
[LEGACY.md](LEGACY.md). They are not current product surfaces.
