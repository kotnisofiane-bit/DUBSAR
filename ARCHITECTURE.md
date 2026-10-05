# DUBSAR Architecture

DUBSAR separates durable work, observations, probabilistic judgment and
authority. Personal and Control Plane are two environments of this common
architecture.

This is a public responsibility and reference-boundary description. It
publishes no private implementation, internal policies, signing material or
deployment topology. [STATUS.md](STATUS.md) defines maturity; the diagrams
below do not assert that every path is integrated or qualified.

## Common responsibility model

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

The downward path is a decision boundary. Execution returns observations to
deterministic software for validation and state updates; it does not let the
agent write its own authoritative account of success.

| Responsibility | Owner | Boundary |
|---|---|---|
| Canonical mission and operational state | Deterministic software | A session, model response or UI projection cannot redefine the mission |
| Evidence records and source status | Deterministic software | Provenance, versions, freshness, coverage and unavailable reads stay explicit |
| Next justified cognitive move | Judgment | A proposal within a closed contract, with no execution authority |
| Permissions and state transitions | Deterministic Core / policy | Validated authorization, independent of prompt wording |
| Consequential effects | Human authority through policy and Human Gates | Approval is attributable and bound to the action under review |
| Execution | Agents, automation and tools | Work occurs only inside admitted scope; results require observation |

Software owns the records and validation rules. It does not make every source
complete or every observed statement true. Missing evidence and uncertainty
remain part of canonical context.

## Durable mission state

A mission must remain identifiable across sessions, handoffs and provider
changes. Its objective, scope, constraints, current state, evidence references,
decisions and unresolved work should be preserved by software.

Conversation history can inform the mission, but cannot replace its canonical
state. Memory carries relevant continuity; Operational Context describes what
is known about the current situation. A generated summary cannot silently
refresh a source or promote an old checkpoint into present success.

Three outcomes remain separate:

- **Execution success:** the bounded operation returned an observed result.
- **Mission success:** the mission's acceptance conditions are supported.
- **Proof:** attributable material supports a specific claim within its limits.

None implies the other two automatically.

## DUBSAR Personal

Personal is the first product expression, built around a Desktop experience:

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

My Work anchors the mission. Agents execute bounded assignments; Hermes is
part of that agent layer rather than the owner of the work. Memory preserves
continuity. Automation and the Tool Layer expose explicit execution contracts
and source access. Operational Context preserves observations, coverage and
evidence references.

Judgment proposes the next cognitive move. Trace Canvas is intended to project
the recorded path, decisions and limits; rendering a trace creates neither
evidence nor permission. Human Gates expose consequential decisions with their
scope, evidence, limitations and expected effects.

All these views should refer to one coherent mission. Users should be able to
change agents or model providers without losing the work itself. Desktop and
Trace Canvas integration, local Judgment and continuity across every view
remain active work, not a public installable release.

## DUBSAR Control Plane

Control Plane uses the same boundaries for heavier or organizational
workloads. The reference execution path is:

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

| Boundary | Required property |
|---|---|
| Human / Core decision | Policy checks the requested scope; required Human Gates remain explicit |
| Signed authorization / Task Lease | Authorization is bound to a workload and a limited scope and lifetime |
| Runtime admission | Deterministic validation decides whether this execution may start |
| Durable handoff | Execution identity and ownership survive interruption and recovery |
| Workload / sandbox | The agent runs inside an admitted execution boundary |
| Mediated egress | Outbound effects can be checked at an enforced boundary |
| Gateway / Broker | Provider access and credentials remain outside the agent |
| Evidence / Operational Context | Observations, failures, uncertainty and outcome references return to governed state |

Authorization is not a prompt instruction. Replay and admission must be
deterministic: a model does not decide whether a lease is valid or an
execution is a duplicate.

Crash recovery must reconcile the durable execution identity before retrying.
A crash must not silently create a second execution. Where an external
effect cannot be established, the state must expose uncertainty rather than
invent successful completion or blindly repeat the effect. This requirement
does not claim universal exactly-once execution across external providers.

The agent does not own provider credentials and cannot approve itself.
Mediated egress requires traffic to pass through the actual enforced
boundary; a diagram or policy statement alone does not mediate a workload.
Complete real-world qualification of every component and of the combined
path is not claimed.

## Judgment contract

Judgment is a bounded probabilistic policy/controller, not a super-agent
orchestrator. Its input is an AgentContext assembled by software from
identified mission state, permitted context, evidence and limitations.

The controller proposes one next cognitive move from a closed set, for
example:

- `consult`: request permitted context or analysis;
- `conclude`: propose a supported conclusion for validation;
- `clarify`: request missing information;
- `revise`: reconsider a proposal within scope;
- `stop`: propose stopping the cognitive path.

These examples are a public vocabulary, not a published API schema. Software
checks the contract, references and applicable authority before execution.
Malformed or unsupported output cannot create an authorized action.

Judgment cannot:

- create a permission;
- create evidence;
- declare a source fresh;
- declare a mission complete without supporting records;
- grant itself authority;
- assert that a real action succeeded.

A `conclude` proposal does not close a mission. A model's confidence does
not upgrade the evidence. Qwen is the current local candidate; providers can
change without changing the authority model.

## Human Gates and policy

A Human Gate binds a decision to the actual scope, state, evidence,
limitations and consequential effect presented for review. An agent's claim
that approval happened is not approval.

Policy can apply previously authorized rules within their scope. It cannot
derive new human authority from a model proposal. Required protected
boundaries stop when authorization or supporting material is missing.

## Public technical source

The [Technical components section](README.md#technical-components) links
available public component source and its limits. This root does not publish
the private Core or claim that other implementation repositories are public.
The earlier RFCs and diagrams are historical references indexed in
[LEGACY.md](LEGACY.md), not current contracts.
