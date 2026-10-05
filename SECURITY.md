# Security Policy

DUBSAR is under active development and is not generally available for production use.

## Supported versions

No public production version is currently supported.

Historical Marketplace or plugin staging files recoverable from Git history are
unsupported and must not be restored or installed in a production environment.

## Reporting a vulnerability

Until a dedicated monitored security channel is confirmed publicly, contact:

`kotni.sofiane@dubsar.ai`

Use `SECURITY` in the subject line and provide only the minimum information required to establish contact.

Do not include:

- credentials or tokens;
- private keys;
- cookies or session material;
- real client evidence;
- personal data;
- exploit code targeting a live third-party system;
- private Core material.

A secure exchange channel can be agreed after initial contact.

## Current public scope

Reports may concern:

- this public documentation repository;
- public marketing website behavior;
- unexpected exposure or access-control failure on a DUBSAR endpoint;
- authentication or authorization boundaries;
- accidental data or secret exposure;
- published adapter staging material.

Private repositories, client environments and third-party services must not be probed without explicit authorization.

## Product security model

DUBSAR is designed around:

- explicit identity;
- bounded evidence collection;
- least-privilege connectors;
- separation of browser, service, agent and human authority;
- deterministic state transitions;
- fail-closed behavior for protected operations;
- visible missing or unavailable evidence;
- private Core isolation;
- expurgated proof artifacts.

These are design requirements. They are not a claim that a public production security review has been completed.

## Personal and Control Plane boundaries

Personal is in active integration / technical development, with no public
installable release. Control Plane's reference execution path is documented
in [Architecture](ARCHITECTURE.md); complete live qualification is not claimed.

Security validation must cover the actual implemented boundaries:

- mission and workspace isolation where applicable;
- connector scope and credential separation from agents;
- deterministic validation of signed authorization / Task Leases;
- admission, replay and durable handoff during failure and recovery;
- workload / sandbox isolation and enforced mediated egress;
- evidence provenance and visible uncertainty;
- authenticated Human Gates bound to the intended consequential effect;
- retention, deletion, logging and recovery;
- dependencies, artifact integrity and update behavior.

These are requirements for the relevant environment, not completed
qualification claims. A model proposal cannot supply authorization or bypass
a required gate. A Gateway mediates only traffic actually routed through its
enforced boundary.

Any public distribution needs security validation for its real data flows,
supported platforms and release artifacts. See [Status](STATUS.md) and
[Installation](INSTALLATION.md).

## Disclosure status

A full vulnerability-disclosure and response SLA will be published before general availability.
