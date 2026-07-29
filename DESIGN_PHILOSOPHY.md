# Design Philosophy

DUBSAR is designed around a practical question:

> How can business automations and AI agents remain understandable, governable and attributable across tools and over time?

The answer is not to ask another agent to declare that everything is safe. It is to combine bounded evidence, deterministic controls, specialized roles and explicit human authority.

## Audit before continuous governance

Responsible orchestration starts by understanding the existing system.

The first product path therefore:

1. defines a bounded scope;
2. collects authorized evidence;
3. freezes a reproducible snapshot;
4. applies explicit controls;
5. exposes findings and missing information;
6. records a human disposition;
7. preserves a traceable report.

Continuous policy enforcement follows only when the audit establishes a justified and testable need.

## Determinism and agents have different jobs

Agents are useful for interpretation, exploration and explanation.

Deterministic components own:

- identity and state transitions;
- evidence digests and scope;
- control vocabulary;
- idempotence;
- protected policy decisions;
- Human Gate enforcement;
- stable report projection.

Model output is input to governance, not governance itself.

## Evidence over confidence

Fluent explanations are useful but insufficient.

DUBSAR keeps observed facts, deterministic results, inferences, missing evidence and unavailable sources distinct. Stronger wording cannot promote an unsupported claim into a verified fact.

## Human responsibility must be usable

Saying “a human remains responsible” is not enough.

The reviewer needs:

- the finding;
- the evidence;
- the rule;
- the scope;
- the limitations;
- the exact review state being decided.

A Human Gate is therefore a bound decision surface, not a decorative checkbox.

## Prefer explicit boundaries

Every audit or governed action should identify:

- objective;
- owner;
- allowed scope;
- prohibited scope;
- evidence requirements;
- active Rule Pack or policy;
- agent role boundaries;
- Human Gate conditions;
- expected output.

Boundaries do not guarantee correctness. They make divergence reviewable.

## Fail closed selectively

A protected action should stop when required identity, evidence, policy or authorization is missing.

Harmless reads should not become unusable through indiscriminate blocking. Fail-closed behavior must protect meaningful boundaries rather than perform security theatre.

## Keep connectors replaceable

n8n, Make, CRM systems, model providers and coding-agent hosts evolve independently.

DUBSAR should use documented, versioned contracts and explicit degraded states. A connector change may require an adapter update; it must not change the meaning of an audit result silently.

## Portal for users, local administration for operators

The portal is the primary surface for scope, findings, review and reports.

A future Node and desktop are intended for technical administrators who need local credentials, runtime health, connector configuration and controlled execution.

These surfaces share one authority model. They do not create separate governance brains.

## Preserve the private authority boundary

Public adapters, schemas and examples can remain inspectable.

Canonical audit state, protected policy and proprietary deterministic mechanisms remain in the private DUBSAR Core. Open-source components in the surrounding system do not make the complete product open source.

## Keep public status honest

An interface, an API test, a deterministic function test, a user E2E and production readiness are different kinds of proof.

Every public claim should name which boundary was actually exercised.

## Developer heritage

Earlier Claude Code, desktop and multi-session work remains useful.

It contributes patterns for identity, evidence, local runtime and Human Gates. Developer adapters are now a secondary experimentation track rather than the primary public product.

## Summary

DUBSAR is not designed to maximize autonomous activity.

It is designed to make automation activity more attributable, bounded, reviewable and governable.
