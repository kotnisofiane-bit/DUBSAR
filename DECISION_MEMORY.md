# Decision Memory

Automations and AI-agent systems do not evolve only through configuration or
code. They evolve through decisions.

A business rule, a rejected option, an approval, a rollback or an accepted risk
can shape an operating process for months. If that reasoning is not preserved,
the next audit or execution starts from a partial account of the system.

DUBSAR treats decision memory as infrastructure.

---

## Conversation history is not governed memory

Conversation history records what was said.

Decision memory records what became meaningful for the governed process.

A conversation may contain drafts, uncertainty, alternatives and abandoned
ideas. Governed memory should preserve the decisions, reasons, constraints,
evidence and human authority that future work depends on.

The goal is not to remember everything.

The goal is to remember what the governed process depends on.

---

## The governed case is the continuity anchor

A DUBSAR audit or governance case needs a persistent identity.

That identity provides the durable context within which scope, source versions,
executions, findings, evidence and Human Gates can be related across time.

When the portal becomes available, a portal session may end. A connector or
Node can restart. The governed case should remain identifiable and its evidence
path reproducible.

---

## What a decision should preserve

A meaningful decision should be relatable to:

- the audit or governance case;
- the business question or intended action;
- the alternatives considered where relevant;
- the chosen decision and reason;
- the rule, policy or constraint it activates or removes;
- the affected system, workflow and business object;
- the relevant execution identity and source versions;
- supporting evidence and its verification level;
- the human decision when a protected action was reviewed;
- later replacement, revision or rollback.

---

## Active, replaced and revised decisions

Decision memory is not a museum of permanent rules.

A decision can be challenged, replaced or reversed. DUBSAR should preserve the transition rather than silently overwrite the past.

Future audits and executions need to know both:

- what is currently authoritative for the governed process;
- how and why that state was reached.

---

## Memory is not authority

Memory does not decide what is correct.

It provides the governed context in which agents can propose and humans can decide. An old decision may no longer apply, but its retirement should be explicit.

---

## Memory connected to work

Decision memory becomes useful when it informs:

- case resumption;
- audit scope and source boundaries;
- workflow and policy selection;
- relevant constraints;
- canonical execution identity;
- expected evidence;
- audit questions;
- Human Gate dossiers;
- replay after retry, restart, handoff or connector change.

It is not a passive archive detached from the workflow.

---

## Evidence and memory are different

A decision record may reference evidence, but the record itself does not prove that the evidence is valid.

DUBSAR distinguishes:

- what was declared;
- what was verified;
- what is missing;
- what is invalid;
- what the human ultimately decided.

This prevents a persuasive narrative from becoming a substitute for proof.

---

## Replayable path

A governed path may be summarized as:

```text
Authorized scope
  → Evidence snapshot
  → Rule and source versions
  → Execution or proposed action
  → Findings and limitations
  → Human review
  → Human Gate
  → Decision and traceable report
```

Replay does not mean storing private chain-of-thought or every token of every
interaction. It means preserving the bounded facts required to explain a result
and resume the governed process.

---

## Questions decision memory should answer

- Why does this constraint exist?
- Which decision is active now?
- What replaced the previous direction?
- Why was this option rejected?
- Which workflow, agent or execution produced this result?
- Which evidence supported the change?
- Was that evidence declared or verified?
- Which human decision authorized protected movement?
- What should the next execution, connector or Node inherit?

---

## Summary

Conversations disappear. Decisions remain.

An organization that preserves governed decisions can evolve its automations and
agents without repeatedly losing the evidence and authority behind them.
