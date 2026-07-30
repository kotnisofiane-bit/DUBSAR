# Installation

There is no supported public installation of DUBSAR at this time.

The public repository no longer contains an active Marketplace manifest or a
vendored Claude Code plugin runtime. Source visibility, documentation or Git
history must not be treated as an installation path.

## Product surfaces

### Automated audit portal

The portal is coming soon and is still under construction and validation. It is
not currently available and does not require a local installation from this
repository.

The public audit method is described at
[dubsar.ai/audit](https://dubsar.ai/audit).

### Professional DUBSAR Audit

The professional audit is available on request as a separately scoped,
human-led engagement. It does not imply that a generally available software
package or local Node has been published.

### DUBSAR for Claude Code

The coding-agent product remains a controlled private beta, selective and
Windows-first. If access is approved, the tester receives a bounded,
version-pinned procedure through the controlled beta channel.

Nothing in this public repository replaces that approved procedure.

## No public install commands

Do not:

- install a plugin from an older Git commit;
- reconstruct the retired `plugins/scribe/` tree;
- copy an unpublished Marketplace manifest into Claude Code;
- mix historical Desktop, runtime, plugin or Backend versions;
- assume that an internal technical identifier such as `scribe` names a second
  public product;
- use staging material in a production or client environment.

## Requirements for an approved beta procedure

Any controlled beta procedure must identify:

- the approved Desktop and local runtime version;
- the approved plugin version and source commit;
- required private Backend/Core compatibility;
- hashes or signatures for distributed artifacts;
- supported operating system and prerequisites;
- credential and secret boundaries;
- clean install, update, rollback and removal steps;
- expected self-check and acceptance evidence;
- a support and incident contact.

A green CI run, a visible source tree or a working internal API is not proof of
a reproducible user installation.

## Future public installation

Public installation instructions will be added only after a new package passes
the distribution gates in [Marketplace and Distribution](MARKETPLACE.md).

Until then:

```text
supported public installation: none
public Marketplace manifest: none
public plugin runtime in this repository: none
automated audit portal: coming soon, not currently available
controlled Claude Code private beta: selective, Windows first
```

See also:

- [Current status](STATUS.md)
- [Security boundary](SECURITY.md)
- [Integrity and provenance](INTEGRITY.md)
- [Historical Marketplace record](docs/legacy/marketplace-0.11.1/README.md)
