# Access and Installation

DUBSAR does not currently provide a supported public installation.

The first product path is browser-based through the DUBSAR Portal. The complete portal audit journey is still being consolidated and public self-service access is not announced.

## Current access boundary

```text
public website: informational
public self-service portal: not announced
supported customer installation: none
local Node package: not released
administration desktop: prototype / roadmap
developer-host adapters: experimental
production-ready release: no
```

Repository visibility does not grant access to the private Backend or Core and does not make the visible plugin staging code a supported product.

## Portal-first journey

The intended initial user path is:

1. create or receive authorized portal access;
2. create an audit project;
3. define a bounded scope;
4. import approved synthetic or client-authorized evidence;
5. run the selected Rule Pack;
6. review proposed findings and source references;
7. record a human decision;
8. access a traceable report.

No external agency or customer should be asked to rely on this journey until the internal browser E2E has been completed and independently reviewed.

## Future local Node

Some client systems cannot or should not expose credentials to a hosted service.

A future DUBSAR Node is intended to run inside the client environment and:

- keep source credentials local;
- make outbound authenticated HTTPS connections;
- collect only the approved evidence scope;
- filter and bound exports;
- submit evidence snapshots to DUBSAR;
- report connector and runtime health.

The Node must not approve findings, bypass the Human Gate or write directly to private Core state.

No supported Node package or command is currently published.

## Future administration desktop

The administration desktop is intended for the client's technical operator, not for every portal user.

Its target responsibilities include:

- Node and connector setup;
- local runtime health;
- approved policy configuration;
- audit and governance observability;
- controlled recovery and diagnostics.

The desktop prototype and earlier Windows packaging work are technical foundations. They do not establish a supported customer installation.

## Developer adapters

This repository contains staging material for a Claude Code adapter under historical `scribe` identifiers.

It is:

- experimental;
- not the primary DUBSAR product;
- not a supported public installation;
- not the final Marketplace publication candidate;
- not proof that Codex or Cursor adapters are available.

Do not install or combine historical packages from older SCRIBE documentation.

## Package provenance

Any future supported package must bind:

- product and component versions;
- source commit;
- package hash;
- supported operating system and architecture;
- compatible portal, Backend and Core contract versions;
- update, rollback and removal behavior;
- security and privacy documentation matching the implemented data flow.

A green CI run or successful local launch is not a user E2E proof.

## Security

Never publish or submit:

- API keys;
- access or refresh tokens;
- source-system credentials;
- cookies or human-authorization proofs;
- private Core material;
- real client evidence in a public issue.

See [SECURITY.md](SECURITY.md) and [PRIVACY.md](PRIVACY.md).

## Availability

Access, installation and design-partner testing will be announced only after the corresponding path is reproducible and reviewed.

For current product status, see [STATUS.md](STATUS.md).
