# DUBSAR

**A control plane for durable, governed agentic work.**

Agents can work. DUBSAR keeps durable mission state, evidence, operational
state, bounded judgment and explicit authority separate from the agent itself.
The work should survive a session ending, a runtime crashing or a change of
agent or model provider.

> The software carries reality.
> The model carries judgment.
> Humans retain authority over consequential effects.

This repository is the **canonical public entry point** for DUBSAR. It is a
technical documentation root, with no application code or installable Personal
release. Development is active; component tests do not establish an integrated
product or general availability.

[Current status](STATUS.md) · [Architecture](ARCHITECTURE.md) ·
[Version française](README.fr.md)

## Why it exists

An agent session can produce a useful result while losing the mission, its
constraints, the evidence behind a decision or the authority to act.
Conversation history and execution logs alone do not preserve that work.

DUBSAR separates what is known, what is proposed, what is authorized and what
actually happened. Execution success, mission success and proof are distinct.
See [Why DUBSAR?](WHY_DUBSAR.md) and [Why not just agents?](WHY_NOT_JUST_AGENTS.md).

## One architecture, two environments

The following is a responsibility model, not a claim that every path is
already integrated:

```text
Facts / State / Evidence
        ↓
Deterministic software
        ↓
Bounded Judgment
        ↓
Explicit authority
        ↓
Agents / Automation / Tools
```

Agents do the work. Deterministic software owns canonical state, permissions
and evidence records. Judgment proposes the next justified cognitive move;
it has no authority. Policy and Human Gates remain authoritative for
consequential effects. Execution observations return through software
validation before they can update canonical state.

### DUBSAR Personal

Personal is the first product expression of this system: a Desktop experience
for durable missions. Its current target architecture is:

```text
Desktop
├─ My Work / durable missions
├─ Agents / Hermes
├─ Memory
├─ Automation
├─ Tool Layer / Connectors
├─ Operational Context / Evidence
├─ Judgment
├─ Trace Canvas
└─ Human Gates
```

Users should be able to change agents or model providers without losing the
work itself. My Work, Memory and traces should refer to the same mission,
rather than create competing accounts of progress.

**Status: active integration / technical development.** Desktop, Trace Canvas,
local Judgment and a coherent mission across all views remain integration
work. This is not an announcement of a public beta, supported platforms or
commercial support.

### DUBSAR Control Plane

Control Plane applies the same state, evidence and authority model to heavier
or organizational agentic workloads. Its reference execution boundary is:

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

The design keeps provider credentials outside the agent, treats authorization
as a validated object rather than a prompt instruction, and requires
deterministic admission and replay decisions. Recovery after a crash must not
silently create a second execution. Egress can be mediated; an agent cannot
approve itself.

This describes component boundaries and integration requirements. It does
not claim that the whole stack is already integrated live or qualified in
every real runtime. [Architecture](ARCHITECTURE.md) details the boundaries.

## Judgment

Judgment is a bounded probabilistic policy/controller. It selects a next
cognitive move from a closed set, for example `consult`, `conclude`,
`clarify`, `revise` or `stop`. It is not a super-agent orchestrator.
Software validates the proposal and executes only authorized actions.

Judgment cannot create permission or evidence, declare a source fresh,
complete a mission without supporting records, grant itself authority or
claim that an action really succeeded. A `conclude` proposal is not mission
completion. Qwen is the current local model candidate, not an architectural
dependency.

## What exists today

Development has working components for durable work state where supported,
deterministic contracts and validators, evidence boundaries and Human Gate
patterns. Automation and AgentContext / Judgment contracts are part of the
technical work. Integration remains active.

[STATUS.md](STATUS.md) separates acquired components, active integration and
claims not yet made. It also distinguishes the project-reported technical
state from what a reader can inspect publicly. No test result is promoted
into a product-release claim.

## Technical components

- [DUBSAR Contracts — reference](https://github.com/kotnisofiane-bit/dubsar-contracts-reference):
  public contracts-and-conformance source with versioned schemas,
  deterministic validators, reference implementations and synthetic tests
  for Operational Context, Judgment boundaries, Task Lease / S1, Broker,
  AgentContext and Automation. It is not the private canonical source, the
  full Control Plane runtime or an installable Personal release.
- Further component repositories will be linked here when their public source
  and scope are available. The private `dubsar-contracts` repository remains
  the canonical development source for this extracted reference publication.

This root remains canonical for the overall project. Earlier audit, skills,
Marketplace and Scribe surfaces are indexed in [LEGACY.md](LEGACY.md);
they do not define current product availability.

## Read further

- [Product surfaces](PRODUCT_SURFACES.md): Personal and Control Plane.
- [Design philosophy](DESIGN_PHILOSOPHY.md) and [Principles](PRINCIPLES.md):
  state, judgment and authority.
- [Roadmap](ROADMAP.md): integration priorities without a release promise.
- [FAQ](FAQ.md), [Installation](INSTALLATION.md), [Security](SECURITY.md),
  [Privacy](PRIVACY.md) and [Rights](RIGHTS.md): public boundaries.

Created by **Sofiane Kotni**.
