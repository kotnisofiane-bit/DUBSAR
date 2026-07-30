# Integrity and Provenance

## Current active tree

The active repository tree contains no public Claude Code Marketplace manifest
and no vendored `plugins/scribe/` runtime.

Therefore, this repository currently exposes no installable plugin artifact
whose integrity can be established from a package hash. Public documentation is
not a distribution package.

## Retired staging snapshot

The previous tree contained an executable staging snapshot with the following
recorded provenance:

| Field | Historical value |
|---|---|
| Product | DUBSAR |
| Technical plugin package | `scribe-bridge` |
| Plugin version | `0.11.1` |
| Private source repository | `kotnisofiane-bit/scribe-claude-code-plugin` |
| Private source commit | `c2878313198aceccac078bf9446c5ab45751e424` |
| Historical vendored tree | 49 tracked plugin files |
| Vendored-tree aggregate SHA-256 | `df9cee3af505c606824edd27485d471a418e75593468426ff10c00501bb0f38f` |
| Active-tree status | Removed; unsupported and not an active distribution artifact |
| Retirement date | 2026-07-30 |

The non-executable tombstone is available at
[`docs/legacy/marketplace-0.11.1/README.md`](docs/legacy/marketplace-0.11.1/README.md).
The earlier bytes and detailed per-file hash list remain recoverable from Git
history for audit purposes.

The historical aggregate hash identifies that earlier vendored tree only. It
does not:

- authenticate a future package;
- approve installation;
- establish compatibility with a current Desktop, Backend or Core;
- establish production readiness;
- replace a dependency, provenance or licence review;
- grant rights to private components.

Because the canonical source repository is private, a person without authorized
source access cannot independently reconstruct the historical snapshot from
this record alone.

## Future distribution requirements

If DUBSAR later publishes a new plugin package, its integrity record must be
generated from the final approved artifact and must include:

1. the public package name, version and canonical source commit;
2. the exact allowlist of distributed files;
3. per-file hashes and an aggregate artifact hash;
4. dependency lock and third-party notices;
5. the applicable reviewed licence information;
6. build or packaging instructions that reproduce the artifact;
7. supported platform and compatibility pins;
8. signature or release-attestation information where available;
9. install, update, rollback and removal validation evidence.

The new record must not reuse the retired `0.11.1` hash.

## Licence boundary

This retirement does not select a public software licence for DUBSAR.

The previous private-beta licence has been moved from the repository root to the
[historical `0.11.1` record](docs/legacy/marketplace-0.11.1/LICENSE.txt). It
describes the retired plugin snapshot and does not decide the licensing of the
Portal, Desktop, Backend, future plugins or any other future distribution.

The active repository's current rights and distribution position is recorded in
[Rights and Licensing Status](RIGHTS.md). Third-party components remain subject
to their own licences and notices.

## Status

```text
active public Marketplace manifest: absent
active vendored plugin runtime: absent
supported public plugin artifact: none
historical v0.11.1 provenance: recorded; bytes removed from the active tree
future publication: requires new provenance, integrity and licence evidence
```
