# Historical DUBSAR Marketplace Staging Record (v0.11.1)

## Status

This directory is a non-executable tombstone.

It contains no plugin code, manifest, archive, command or installation material.
The corresponding Marketplace staging surface was retired from the active
repository tree on 2026-07-30.

It is not:

- a supported DUBSAR release;
- an installable Claude Code plugin;
- an active Marketplace source;
- a production artifact;
- a licence grant for private DUBSAR components.

## Recorded provenance

| Field | Historical value |
|---|---|
| Product | DUBSAR |
| Technical plugin package | `scribe-bridge` |
| Plugin version | `0.11.1` |
| Private source repository | `kotnisofiane-bit/scribe-claude-code-plugin` |
| Private source commit | `c2878313198aceccac078bf9446c5ab45751e424` |
| Historical vendored tree | 49 tracked plugin files |
| Historical vendored-tree aggregate SHA-256 | `df9cee3af505c606824edd27485d471a418e75593468426ff10c00501bb0f38f` |
| Retired active paths | `.claude-plugin/marketplace.json`, `plugins/scribe/` |
| Retirement date | 2026-07-30 |

The aggregate hash applies only to the earlier vendored plugin tree. It does not
cover this tombstone and must not be reused for a future package.

The source repository is private. This recorded provenance is therefore not an
independently reproducible public build recipe.

## Historical licence record

The exact private-beta licence text that accompanied the retired `0.11.x`
plugin snapshot is preserved at [`LICENSE.txt`](LICENSE.txt).

It is retained as historical evidence and is no longer the repository-root
licence. Moving the text does not rewrite Git history, retroactively change
earlier terms or select a licence for any current or future DUBSAR component.
The contact information inside that file is preserved verbatim as part of the
record and is not presented here as the current support channel.

## Why it was retired

The snapshot was an earlier private-beta staging pin, not the final DUBSAR
distribution candidate. Leaving an executable manifest and plugin tree in the
default branch made an unsupported installation path discoverable and blurred
the current product boundary.

The current repository keeps the product doctrine and public evidence while the
coding-agent product remains a controlled private beta.

## Historical recovery

The former files and their detailed per-file hashes remain available in Git
history for authorized audit or forensic comparison. They must not be restored,
copied or installed as a current product package.

Any future Marketplace release must be built from a newly approved source pin
and receive its own provenance, integrity, dependency, licence, security and
installation review.
