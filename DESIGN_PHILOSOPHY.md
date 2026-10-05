# Design Philosophy

DUBSAR is designed around work that survives sessions and remains accountable
when agents, models and tools change.

> The software carries reality.
> The model carries judgment.
> Humans retain authority over consequential effects.

## Preserve continuity in software

The mission, its state, evidence references and decisions should outlive
the agent. Memory should preserve relevant continuity without turning every
conversation into authoritative knowledge.

Personal views should project one coherent mission. Trace Canvas should
show recorded events and limits, not generate a new account of reality.
Changing a provider should not require abandoning the work.

## Bound probabilistic judgment

Judgment proposes a next cognitive move from a closed vocabulary, using
AgentContext prepared by software. A proposal must pass deterministic
validation before any authorized execution.

Judgment cannot create permission, evidence, freshness or completion.
Its model can change without changing that contract.

## Make authority concrete

Signed permissions / Task Leases and runtime admission belong to software
boundaries, not prompt instructions. Human Gates bind consequential decisions
to the scope, state, evidence and effects presented for review.

Policy operates within authorized rules. Neither an agent nor Judgment may
manufacture approval.

## Keep uncertainty visible

Observed facts, inferences, declarations, missing evidence and unavailable
sources remain distinct. Successful execution does not imply mission success
or proof. A crash with an uncertain external outcome needs reconciliation,
not an invented result or a silent duplicate execution.

## Fail closed at meaningful boundaries

A protected action stops when required authorization or evidence is absent.
Harmless reads should remain usable within their allowed scope.

A Gateway or Broker mediates only traffic that actually passes through its
enforced boundary. Provider credentials should remain outside the agent.

## Prefer replaceable contracts

Agents, model providers and connectors evolve independently. Documented
contracts, explicit degraded states and visible coverage limits keep that
change from silently redefining a mission or a permission.

## Keep public claims tied to their scope

A validator test, component E2E, integrated mission and qualified production
runtime are different achievements. [STATUS.md](STATUS.md) separates them.

The current architecture is described in [ARCHITECTURE.md](ARCHITECTURE.md).
Earlier audit and coding-agent reasoning remains in [LEGACY.md](LEGACY.md);
it does not decide current availability or future component licences.
