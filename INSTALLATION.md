# Installation

There is no supported public installation of the DUBSAR product at this time.

This repository is a public documentation boundary. It does not contain the
Portal, private Core, private product implementation or an installable DUBSAR
runtime. Source visibility, documentation and Git history must not be treated
as an installation path.

## Current product access

### Automated audit portal

The portal is coming soon and remains under construction and validation. It is
not currently publicly available and does not require a local installation
from this repository.

The public method is described at
[dubsar.ai/audit](https://dubsar.ai/audit).

### Professional DUBSAR Audit

The professional audit is available on request as a separately scoped,
human-led engagement. It does not imply that a generally available software
package or installed component has been published.

## Separate public skills

The
[dubsar-agent-skills](https://github.com/kotnisofiane-bit/dubsar-agent-skills)
repository publishes MIT-licensed doctrine and bounded local helpers. Follow
that repository's own README and licence for those files.

Installing or copying those skills:

- is not an installation of the DUBSAR product;
- does not include the Portal, private Core, private implementation or runtime;
- does not grant access to private DUBSAR services;
- does not activate a public DUBSAR beta.

The skills repository's MIT licence does not apply to this repository or to
private DUBSAR components.

## No public product install commands

Do not:

- install a plugin from an older Git commit;
- reconstruct the retired `plugins/scribe/` tree;
- copy an unpublished Marketplace manifest into a host;
- mix historical Desktop, runtime, plugin or Backend versions;
- assume that an internal identifier such as `scribe` names a current public
  product;
- use staging material in a production or client environment.

## Future distribution

Any future software distribution will require a new, component-specific
decision and review. At minimum, it must define:

- the exact distributed component and canonical source;
- its licence and third-party notices;
- supported platforms and compatibility;
- artifact integrity and provenance;
- credential, privacy and security boundaries;
- clean installation, update, rollback and removal;
- acceptance evidence and support boundaries.

No future DUBSAR software publication is promised by this document.

```text
supported public DUBSAR installation: none
public DUBSAR Marketplace manifest: none
public DUBSAR plugin or runtime in this repository: none
automated audit portal: coming soon, not currently available
professional DUBSAR Audit: available on request
public skills: separate MIT-licensed companion resource
```

See also:

- [Current status](STATUS.md)
- [Rights and licensing status](RIGHTS.md)
- [Security boundary](SECURITY.md)
- [Integrity and provenance](INTEGRITY.md)
- [Historical Marketplace record](docs/legacy/marketplace-0.11.1/README.md)
