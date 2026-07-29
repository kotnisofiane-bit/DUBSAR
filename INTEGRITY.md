# Integrity and Provenance

DUBSAR treats provenance as part of the product contract.

## Current repository status

This repository contains public documentation and historical developer-adapter staging material.

There is currently:

- no supported public DUBSAR release;
- no approved Marketplace package;
- no final public adapter pin;
- no production package whose integrity can be asserted from this repository.

Historical hashes or source pins must not be interpreted as current release provenance.

## Release requirements

Every future public package must provide:

- product and component version;
- source repository boundary;
- exact source commit;
- package digest;
- per-file or signed manifest where appropriate;
- build environment and reproducible-build limitations;
- supported platform and contract versions;
- applicable licence and third-party notices;
- publication date and release status.

The published manifest must describe the exact bytes distributed to users.

## Evidence integrity

Audit evidence has a separate integrity boundary.

An audit should preserve:

- source kind and authorized scope;
- collection window;
- source or projection digest;
- completeness and unavailable reads;
- immutable run association;
- Rule Pack identity and declared digest;
- finding-to-evidence references;
- review and report identity.

A digest proves that content has not changed relative to that digest. It does not, by itself, prove that the content is true, complete, legally sufficient or approved by the Core.

## Public verification material

When a real public release exists, this file may link to:

- detached checksums;
- signed provenance;
- software bill of materials;
- reproducible verification instructions;
- release-specific third-party notices.

Until then, no historical staging command should be presented as a canonical verification path.

## Private boundary

Public provenance must not expose:

- private repository access paths;
- internal deployment topology;
- secrets, tokens or signing material;
- confidential proof archives;
- private Core implementation;
- client or tester data.

## Reporting an integrity problem

Use the process in [SECURITY.md](SECURITY.md). Never include credentials or private evidence in a public issue.
