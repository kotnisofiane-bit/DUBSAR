# Marketplace and Distribution

## Current decision

DUBSAR does not currently publish a Claude Code Marketplace package or any
other public product package.

The historical staging manifest and vendored `plugins/scribe/` runtime have
been retired from the active repository tree. There is no supported public
installation command, Marketplace source, plugin archive, beta-access path or
self-service update path in this repository.

The current direction is Personal and Control Plane, documented in
[README.md](README.md) and [STATUS.md](STATUS.md). Earlier audit offers,
Claude Code packaging and public-skills positioning are historical phases.

## Public components

Available component source is listed under
[Technical components](README.md#technical-components). It is separate from
this retired Marketplace surface and from an installable Personal release.
The historical skills name and its changed destination are recorded in
[LEGACY.md](LEGACY.md).

## Why the staging surface was retired

The visible staging surface could be discovered as if it were installable even
though it was not a final product package. It also combined:

- an earlier private-source pin;
- historical `scribe` identifiers;
- an executable plugin tree;
- Marketplace metadata;
- historical licence terms that now belong only to the retired record.

Keeping that surface in the default branch created ambiguity. The active
repository now documents the public/private boundary without exposing an
obsolete installation candidate.

## Historical record

The retired staging snapshot is recorded, but not redistributed, at
[`docs/legacy/marketplace-0.11.1/README.md`](docs/legacy/marketplace-0.11.1/README.md).

The record preserves:

- historical plugin version `0.11.1`;
- private source commit
  `c2878313198aceccac078bf9446c5ab45751e424`;
- historical vendored-tree aggregate SHA-256
  `df9cee3af505c606824edd27485d471a418e75593468426ff10c00501bb0f38f`;
- the retirement date and scope;
- the historical licence text in its archival location.

Git history preserves earlier bytes. They are not a supported package and must
not be copied from history for installation or production use. The archival
record does not select or grant a current licence for any DUBSAR component.

## If distribution is considered later

Any future publication must be a new, explicit component-specific decision. It
must not reactivate the retired snapshot by default.

Before publication:

1. identify the exact component, canonical source and version;
2. complete dependency, provenance and licence review;
3. define compatibility and support boundaries;
4. generate minimal artifacts from approved source;
5. produce integrity evidence;
6. validate clean installation, update, rollback and removal on every claimed
   platform;
7. publish accurate security, privacy and data-boundary information;
8. obtain explicit approval for distribution.

No future Marketplace publication is promised or scheduled here.

## Status

```text
public DUBSAR Marketplace: retired from the active tree
supported public DUBSAR installation: none
historical staging version: 0.11.1, record only
active coding-agent beta: none
current product direction: Personal / Control Plane in development
future product distribution: undecided; requires a new reviewed decision
```
