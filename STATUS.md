# Status

DUBSAR is in active technical development and integration as a control plane
for durable, governed agentic work. Personal is its first product expression;
Control Plane applies the same architecture to heavier workloads.

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

The publicly inspectable component currently linked is
[DUBSAR Memory](https://github.com/kotnisofiane-bit/dubsar-memory), a technical
preview of durable project memory, a CLI and a read-only Workbench.
That repository defines its own tests, limits and licence. Its memory
contracts do not prove integrated Judgment, runtime admission or egress.

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
- complete real-world runtime qualification of every Control Plane component;
- universal connector, agent-host or operating-system support;
- a public `dubsar-contracts` repository or distribution of the private Core.

## What would justify stronger claims

An integration claim needs a reproducible path tied to component versions,
the tested environment and retained results. Mission recovery, rejected
authorization, retries, partial evidence and required Human Gates must remain
observable. Execution success must stay separate from mission completion.

A public release also needs an actual artifact, installation and removal
validation, supported environments, licensing, security and privacy boundaries.
No release date or access invitation is announced here.

## Repository boundary

This repository is documentation only. [Installation](INSTALLATION.md) and
[Rights](RIGHTS.md) define its distribution and licensing boundary.
[LEGACY.md](LEGACY.md) indexes the earlier audit and coding-agent phases;
their old availability statements are historical.
