# Developer Adapters and Marketplace Boundary

The DUBSAR product is now portal-first. Claude Code, Codex and Cursor integrations remain secondary developer-adapter work.

## Important warning

> The Marketplace metadata and vendored plugin currently present in this repository are historical staging material. They are not a supported installation path, not the current product, and not the final publication candidate.

Do not add this repository as a Marketplace, install the staged adapter or combine it with historical SCRIBE packages.

## Why the staging material remains visible

The project previously explored DUBSAR primarily as a governance plugin for coding-agent hosts.

That work produced useful foundations:

- explicit session identity;
- bounded commands and tools;
- evidence capture;
- decision memory;
- Human Gates;
- multi-session experiments.

The product direction has since broadened. The primary customer path is now an audit and governance portal for business automations and AI agents.

The staging material remains visible temporarily for provenance and review. Its presence is not an availability announcement.

## Known publication blockers

Before any developer adapter can be announced:

1. complete the repository and licence audit;
2. reconcile third-party notices and component licences;
3. remove or migrate the historical generic-session fallback;
4. select one canonical adapter source and commit;
5. remove private or obsolete repository links;
6. align package, plugin and repository licence metadata;
7. verify the adapter against the current Backend and Core contracts;
8. prove clean install, update, rollback and removal;
9. document supported host and operating-system versions;
10. publish integrity information for the exact release;
11. complete an external user journey without hidden operator repair;
12. obtain explicit human approval to publish.

## Current adapter status

| Surface | Status |
|---|---|
| Claude Code staging adapter | Historical private-beta experiment; unsupported |
| Public Claude Marketplace | Not activated or announced |
| Codex adapter | Exploration / roadmap |
| Cursor adapter | Exploration / roadmap |
| Local administration Node/Desktop | Separate prototype and roadmap |
| Portal audit | Primary product path, internal validation |

## Relationship to the primary product

A future developer adapter may:

- identify a host session;
- submit bounded evidence;
- receive governed state;
- surface a required Human Gate;
- connect a development workflow to DUBSAR policy.

It must not:

- contain or replace the private Core;
- let an agent approve its own work;
- hide missing evidence;
- bypass portal or Core authority;
- imply that the complete DUBSAR product is open source.

## Historical identifiers

Staging files may contain identifiers such as:

- `scribe-bridge`;
- `scribe-mcp`;
- `/scribe-*`;
- `scribe.*`;
- `SCRIBE_*`.

They are historical compatibility identifiers. They are not a second current product and must not be renamed through an untested global replacement.

## Distribution boundary

A future public adapter package may contain only:

- the approved thin host adapter;
- required public metadata;
- its applicable licence and third-party notices;
- bounded public documentation;
- release integrity information.

It must not contain:

- the private Core;
- private Backend implementation;
- internal prompts or policies;
- private tests or proof archives;
- credentials, tokens or trust material;
- client or tester data.

## No installation command

There is currently no supported public command for installing a DUBSAR developer adapter.

See [INSTALLATION.md](INSTALLATION.md) and [STATUS.md](STATUS.md) for the current boundary.
