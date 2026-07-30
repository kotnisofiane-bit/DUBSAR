# Why Not Just Agents?

AI agents are useful. Multi-agent systems can divide work, use tools and move quickly.

DUBSAR is being built as an audit and governance layer. It can orchestrate
bounded roles, but it does not make another model the final authority over
those agents.

## Agent activity is not governance

A group of agents can still:

- repeat the same action;
- use incompatible business state;
- lose the rule or version that triggered an action;
- cite incomplete evidence;
- approve its own output;
- hide disagreement behind a fluent summary;
- become impossible to reconstruct later.

More roles do not automatically create traceability, separation of authority or deterministic control.

## Deterministic orchestration

DUBSAR separates two kinds of work.

Agents are useful for:

- interpreting bounded material;
- explaining a proposed finding;
- exploring hypotheses;
- preparing a review;
- carrying out an explicitly authorized role.

Deterministic components are required for:

- identity and state transitions;
- evidence digests and scope;
- rule-pack selection;
- control execution;
- idempotence;
- contradiction handling;
- Human Gate enforcement;
- report projection.

```text
agents propose and explain
deterministic controls preserve the rules
the Core preserves canonical state
humans decide protected movement
```

## Why Hermes?

Hermes provides a flexible open agent runtime and specialized roles.

Within DUBSAR, a Hermes role receives a closed objective, explicit evidence and a required output contract. It does not own the Mission, alter the evidence snapshot or create an authoritative decision.

The value is not the role name itself. The value is the combination of:

- bounded role;
- attributable session;
- explicit evidence;
- deterministic control;
- independent human review.

## Why not only n8n, Make or a coding-agent host?

Existing automation and agent platforms execute useful workflows. They also expose their own logs and controls.

DUBSAR is intended to work across those surfaces:

- compare execution with business state;
- preserve an independent evidence snapshot;
- apply controls that are not tied to one vendor;
- keep human decisions and limitations visible;
- continue governing when several automation systems coexist.

DUBSAR does not need to replace every workflow engine to provide that layer.

## Audit before orchestration

The intended first product path is an audit.

Audit establishes:

- which systems and workflows exist;
- what evidence is available;
- where inconsistencies appear;
- which actions are sensitive;
- which owners and validations matter;
- which parts are not evaluable.

Only after this baseline can continuous orchestration or policy enforcement be configured responsibly.

The automated portal implementing this journey is coming soon and remains
under development and validation. It is not currently available for public
use. Professional DUBSAR Audit remains available on request; continuous
governance through a local Node is not generally available.

## Human authority

A human decision is not a ceremonial confirmation after the agents agree.

The reviewer must see the finding, evidence, rule, scope and limitations. The decision can confirm, correct or reject the proposal.

It cannot turn missing evidence into verified evidence and it cannot be manufactured by another agent.

## Summary

DUBSAR uses agents, but does not ask agents to be their own constitution.

It combines agent capabilities with deterministic controls, evidence boundaries, private canonical state and explicit human authority.
