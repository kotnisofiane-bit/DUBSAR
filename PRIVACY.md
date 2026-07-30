# Privacy Boundary

This document describes the current public-information and pre-release boundary
and the privacy questions that must be resolved before broader production use.

It is not yet a final production privacy notice.

## Current availability

The DUBSAR marketing website is publicly accessible. The automated audit portal
is coming soon and is not currently available for public use; development and
validation remain in progress. Professional DUBSAR Audit is available on
request.

The public website provides product information and does not provide access to
the portal. DUBSAR for coding agents remains a controlled private beta. No
generally available connector package, local Node or production desktop is
announced from this repository.

## Data-minimization principle

DUBSAR should collect the smallest evidence scope required for an explicit audit mandate.

The intended model favors:

- metadata over unrestricted content;
- bounded windows over unlimited history;
- explicit source allowlists;
- structured facts over raw payload retention;
- digests and references where content is not required;
- visible exclusions and unavailable reads;
- synthetic fixtures for internal testing.

## Portal accounts

A production portal privacy notice must document:

- account identifiers and authentication provider;
- tenant and project membership;
- access and decision logs;
- support and security communications;
- account closure and deletion;
- retention periods;
- infrastructure and subprocessors.

Registration or public portal access must not be presented as available until
these elements match the deployed implementation.

## Audit imports

An audit may require bounded exports from automation and business systems.

Before a user submits evidence, the product must identify:

- which source is being provided;
- the authorized purpose and scope;
- the expected fields;
- the collection window;
- whether raw content is retained;
- retention and deletion behavior;
- who can review the result;
- known limitations.

Raw credentials, API keys and unrestricted mailbox or conversation archives must not be included in a normal audit import.

## Connectors

Future connectors should use least-privilege access and request only the capabilities required for the selected Rule Pack.

Connector credentials should:

- remain in an approved secret store;
- never appear in findings, reports or logs;
- be revocable;
- have explicit scope and ownership;
- be separated from human-review authority.

For a future local Node, source credentials are intended to stay inside the client environment.

## Models and Hermes

Before broader production use, DUBSAR must document:

- which model or agent providers process which fields;
- whether provider training is enabled or disabled;
- regional and retention behavior;
- redaction and prompt boundaries;
- what remains deterministic;
- how agent outputs are separated from authoritative state.

No model output should silently expand the evidence scope.

## Evidence and reports

Audit records may include:

- source references;
- normalized facts;
- content digests;
- proposed findings;
- reviewer comments and decisions;
- limitations;
- report artifacts.

The production policy must define retention, access, export and deletion for each category.

## Infrastructure

The final notice must match the real deployed providers and data flows, including hosting, routing, storage, authentication, observability and model services.

An architectural intention is not a substitute for a verified data map.

## AI Act and other regulation

DUBSAR may help document provenance, traceability and human oversight.

It does not certify legal compliance and this document does not replace legal advice, a data-protection impact assessment or client-specific contractual review.

## Public repositories

Never publish:

- real audit exports;
- client identifiers;
- access tokens or cookies;
- human-authorization proofs;
- unredacted logs;
- private reports;
- confidential prompts or policies.

Public examples should use synthetic data.

## Before broader production use

Required work includes:

1. verify the deployed data flow;
2. complete the licence and third-party attribution audit;
3. define retention and deletion;
4. define subprocessors and regional boundaries;
5. validate tenant isolation and access controls;
6. publish the applicable privacy notice and terms;
7. establish data-processing agreements where required;
8. test export and deletion behavior.
