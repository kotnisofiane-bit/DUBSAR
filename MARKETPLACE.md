# Marketplace and Distribution

## Current decision

DUBSAR does not currently publish a Claude Code Marketplace package.

The historical staging manifest and vendored `plugins/scribe/` runtime have been
retired from the active repository tree. There is no supported public
installation command, Marketplace source, plugin archive or self-service update
path in this repository.

This decision applies only to public package distribution. It does not change
the status of:

- the public DUBSAR marketing website and documentation;
- the automated audit portal, which is coming soon and is not yet publicly
  available;
- the Professional DUBSAR Audit, available on request;
- the controlled DUBSAR for Claude Code private beta, available only through an
  explicitly approved test path.

## Why the staging surface was retired

The visible staging surface could be discovered as if it were installable even
though it was not the final product package. It also combined:

- an earlier private-source pin;
- historical `scribe` identifiers;
- an executable plugin tree;
- Marketplace metadata;
- conflicting historical licence signals, now preserved only with the retired
  record. Any future public distribution requires a new component-specific
  licence review.

Keeping that surface in the default branch created more ambiguity than useful
product evidence. The active repository now documents the product boundary
without exposing an obsolete installation candidate.

## Historical record

The retired staging snapshot is recorded, but not redistributed, at
[`docs/legacy/marketplace-0.11.1/README.md`](docs/legacy/marketplace-0.11.1/README.md).

The record preserves:

- historical plugin version `0.11.1`;
- private source commit
  `c2878313198aceccac078bf9446c5ab45751e424`;
- historical vendored-tree aggregate SHA-256
  `df9cee3af505c606824edd27485d471a418e75593468426ff10c00501bb0f38f`;
- the retirement date and scope.

Git history preserves the previous bytes. They are not a supported package and
must not be copied from history for installation or production use.

## Conditions for any future Marketplace publication

A future Marketplace surface must be created deliberately from the then-current
product boundary. It must not reactivate the retired snapshot by default.

Before publication:

1. select one approved canonical plugin commit and version;
2. define the public package name and compatibility policy;
3. complete dependency, provenance and licence review;
4. generate a minimal distribution from the approved source;
5. regenerate per-file and aggregate integrity evidence;
6. validate clean install, update, rollback and removal on every claimed
   platform;
7. prove the complete private-beta tester journey without hidden operator
   intervention;
8. publish accurate security, privacy, support and data-boundary information;
9. obtain an explicit Human GO for distribution.

## Status

```text
public Marketplace: retired from the active tree
supported public installation: none
historical staging version: 0.11.1, record only
controlled Claude Code private beta: selective, Windows first
future Marketplace publication: requires a new reviewed package and Human GO
```
