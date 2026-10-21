# Status

DUBSAR is developing a governance foundation with a B2B priority: integrators
and teams deploying AI agents for their clients. Durable mission state,
explicit authorisations, human decisions and execution evidence are intended
to support handover and resumption, including when outcomes remain uncertain.
The [public overview](https://dubsar.ai/en/) describes that direction.

The product remains in active technical development. Full B2B integration and
validation are still underway; pilots are not currently open. Personal remains
the first product expression, and Control Plane applies the same architecture
to heavier workloads. This priority changes neither their boundaries nor the
technical sequence in the [roadmap](ROADMAP.md).

This is the canonical project status as of this public realignment. The
technical categories below reflect the project state supplied for this update.
Private components and their qualification artifacts have not been
independently audited through this documentation repository.

## Acquired / working components

At component scope, where supported:

- durable mission / work state, with recorded checkpoints and resumption;
- deterministic contracts and validators;
- Operational Context / evidence boundaries that distinguish observations,
  declarations, inferences and missing sources;
- Human Gate patterns that separate proposals from protected authority;
- automation integration work at component scope;
- AgentContext / Judgment contracts that bound model input and proposals;
- technical component tests and E2E qualifications where they actually exist.

These items describe technical foundations, not a fully integrated product.
A component E2E qualification applies only to its exercised path and
environment. It does not qualify every Personal view or Control Plane runtime.
This root contains no executable tests or private qualification artifacts.

The publicly inspectable technical source currently linked is
[DUBSAR Contracts — reference](https://github.com/kotnisofiane-bit/dubsar-contracts-reference),
a contracts-and-conformance repository containing versioned schemas,
deterministic validators, selected reference implementations and synthetic
tests. Its own README defines what those suites prove and what they do not.
It is not the private canonical source, an integrated Personal release or the
complete Control Plane runtime.

## In active integration

- a unified Personal experience;
- Desktop integration;
- Trace Canvas integration;
- the local Judgment model, with Qwen as the current candidate;
- provider and connector breadth;
- one coherent mission across My Work, Agents, Memory, Automation, evidence,
  Judgment, traces and Human Gates;
- qualification of the Control Plane execution path across admission,
  handoff, sandbox, mediated egress and evidence collection.

The architecture documents required boundaries; they do not declare the whole
stack integrated live. An individual demonstration or successful test cannot
establish the maturity of the remaining paths.

## Not yet claimed

- a public installable Personal release;
- a public Personal beta or commercial support offer;
- a production-ready enterprise platform;
- general availability;
- complete B2B qualification or open pilots;
- complete real-world runtime qualification of every Control Plane component;
- universal connector, agent-host or operating-system support;
- publication of the private canonical `dubsar-contracts` development
  repository or distribution of the private Core.

## What would justify stronger claims

An integration claim needs a reproducible path tied to component versions,
the tested environment and retained results. Mission recovery, rejected
authorisation, retries, partial evidence and required Human Gates must remain
observable. Execution success must stay separate from mission completion.
An acknowledgement of a request does not establish that its intended effect
occurred; an unresolved outcome must remain explicit for handover and recovery.

A public release also needs an actual artifact, installation and removal
validation, supported environments, licensing, security and privacy boundaries.
No release date or access invitation is announced here.

## Repository boundary

This repository is documentation only. [Installation](INSTALLATION.md) and
[Rights](RIGHTS.md) define its distribution and licensing boundary.
[LEGACY.md](LEGACY.md) indexes the earlier audit and coding-agent phases;
their old availability statements are historical.
