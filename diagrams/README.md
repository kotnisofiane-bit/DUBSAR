# DUBSAR Diagrams

The SVG files currently stored in this folder document an earlier developer-first product direction:

- coding-agent host adapters;
- multi-session development governance;
- a Windows private-beta installation journey.

They remain useful historical design material, but they are **not the canonical diagrams for the current portal-first product direction**.

## Current architecture

The current public architecture is maintained as Mermaid in:

- [`../README.md`](../README.md);
- [`../README.fr.md`](../README.fr.md);
- [`../ARCHITECTURE.md`](../ARCHITECTURE.md).

It describes:

```text
authorized sources
→ DUBSAR Portal
→ bounded evidence snapshot
→ deterministic orchestration and private Core
↔ bounded Hermes roles
→ human review
→ traceable report
```

## Historical diagrams

The existing files should be treated as historical until they are redrawn or moved to an explicit legacy area:

- `dubsar-architecture.svg`;
- `dubsar-architecture-fr.svg`;
- `dubsar-multi-session.svg`;
- `dubsar-multi-session-fr.svg`;
- `dubsar-windows-journey.svg`.

Their presence does not establish:

- a supported Claude Code product;
- a generally available Windows package;
- a working customer desktop;
- current Marketplace availability;
- production readiness.

## Next visual update

The next canonical visual set should cover:

1. portal audit journey;
2. deterministic Core and Hermes role separation;
3. Human Gate and report;
4. future Node and continuous-governance boundary;
5. portal-user versus technical-administrator surfaces.

No private routes, credentials, policies, proof archives or deployment topology should appear in public diagrams.
