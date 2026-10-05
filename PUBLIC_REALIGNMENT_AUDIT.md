# Public Realignment 01 — Documentation Audit

## Scope and source

Repository: `kotnisofiane-bit/DUBSAR`.
Observed base: `main`, `68578b7d9ef4702c8f1c1abe13e66a8851c6d99c`.

The required root documents were read in full, along with the remaining root
pages and the documentation in `docs/`, `examples/`, `rfcs/` and `brand/`.
The repository contains no application code, package manifest, tests or CI.
Public GitHub links and the accessible audit pages of the website were inspected.

The current technical categories come from the project state supplied for
this realignment. Private code and qualification artifacts were not audited.
The public Memory README was checked for its actual component scope.
This is a documentation audit, not a new product qualification.

## Findings before modification

| Classification | Finding | Treatment |
|---|---|---|
| Still valid | Evidence provenance, visible limitations, deterministic state, non-authoritative agents and Human Gates | Retained under the common mission / authority model |
| Useful history | Portal-first audit methods, Scribe / coding-agent work, Marketplace pin and licence, conceptual RFCs | Preserved in marked historical pages and the Legacy index |
| Misleading today | README, Status, Architecture, surfaces, roadmap and FAQ made the audit the current product; installation, security and privacy repeated it | Realigned with Personal / Control Plane and current integration limits |
| Redirected link | `dubsar-agent-skills` resolves to `dubsar-memory` | Removed obsolete skills links and labels; linked the real Memory preview separately |
| Reachable but outdated | `dubsar-docs` still describes the portal-first public direction | Removed from primary navigation; retained with an explicit historical caveat |
| Repetition | Audit journeys, professional offers, AI Act copy, public-skills descriptions and availability tables repeated across root pages | Centralized status in Status, boundaries in Architecture, history in Legacy |

## Resulting public position

DUBSAR is the canonical public entry point for a control plane for durable,
governed agentic work. Personal is the first product expression. Control Plane
addresses heavier workloads under the same state, evidence and authority
architecture.

Judgment proposes bounded cognitive moves and has no authority. Software
validates state, evidence and permissions; humans retain authority over
consequential effects.

The root remains documentation only. No Personal installer, beta, private
source publication, synthetic product canvas or runtime code was added.

## Validation and review boundary

Local validation covers relative links, heading anchors, Markdown structure,
obsolete wording and patch whitespace. Public GitHub component links are
checked against their actual destination and scope. These checks validate
documentation, not product behavior.

On 2026-10-05, the local check resolved all 145 relative references and seven
heading anchors across the Markdown tree, with no errors. Patch whitespace
validation passed. The obsolete-expression review found only explicitly
historical occurrences; no old skills URL remains as an active link.

Historical artwork remains unchanged and is marked in `brand/README.md`;
neither README embeds it. Marketplace provenance and the historical licence
are preserved.

A draft PR is the review artifact. No merge, visibility change, other-repository
mutation or website mutation is included.

## Remaining external contradictions and separate follow-up

- DUBSAR's GitHub description and topics still emphasize audit and AI Act.
  Repository settings are outside this file-only PR.
- The existing GitHub social preview may still use historical artwork;
  replacing that setting needs a separate asset/settings update.
- `dubsar-docs` and `docs.dubsar.ai` retain the earlier product narrative.
- [English audit page](https://dubsar.ai/audit/) and
  [French audit page](https://dubsar.ai/fr/audit) still center the first-product
  story on Flash Audit and refer to a private portal and public Agent Skills.
- Home and product-page inspection through the web tool was unavailable.
  Their copy and navigation need a separate review; no findings about their
  current wording are asserted here.

For the website lot: introduce Personal / Control Plane under one architecture,
align access and maturity with Status, reclassify audit / readiness pages,
correct skills and technical-source navigation, and align EN / FR copy.
No website or companion-repository changes were made.

## Historical R3 record

The earlier record below is retained for provenance. All its “current” claims,
availability statements, references and sequencing belong to the superseded
portal-first phase. Current README, Status and Architecture take precedence.

<details>
<summary>Historical portal-first public alignment audit — R3</summary>

# Historical Public Alignment Audit — R3

## Scope

This audit records the public-documentation boundary after DUBSAR refocused on:

1. the automated audit portal, under construction and coming soon;
2. the Professional DUBSAR Audit, available on request.

It covers positioning, surfaces, status, architecture, roadmap, installation,
Marketplace history, public skills and the public/private boundary. It does not
publish or independently audit private implementation.

Earlier R2 positioning around a coding-agent private beta is superseded by this
record and remains relevant only as project history.

## Executive verdict

The current public story is:

- audit and evidence first;
- explicit limitations and source coverage;
- bounded agent assistance;
- deterministic controls kept distinct from model explanations;
- human review for protected conclusions;
- no automatic legal or regulatory compliance verdict.

The portal and professional service share this doctrine but have different
availability states.

## Current surfaces

| Surface | Public claim |
|---|---|
| Automated audit portal | Coming soon; under construction and validation; not publicly available |
| Professional DUBSAR Audit | Available on request under an agreed mandate |

Continuous governance or installed components may be considered later under a
separate scope. Their architecture, distribution, support and licensing are
undecided and not promised.

## Public skills boundary

The separate
`dubsar-agent-skills` (historical name; see [Legacy](LEGACY.md))
repository contains MIT-licensed public doctrine and bounded local helpers.

It is not the DUBSAR product, Portal, private Core or private implementation.
It grants no access to private services, does not constitute a DUBSAR
installation and does not prove product availability. Its MIT licence applies
only to that repository.

## Historical coding-agent boundary

Earlier DUBSAR experiments explored coding-agent project governance and a
Claude Code Marketplace staging package. They informed the current doctrine but
are paused as a product direction.

Current claims are deliberately limited:

- no current coding-agent commercial surface;
- no active public or private beta;
- no supported Claude Code, Codex or Cursor integration;
- no public plugin, runtime or supported installation;
- historical Marketplace staging retired from the active tree;
- non-executable tombstone retained for provenance only.

## Public/private and licensing boundary

This repository remains public documentation, not a software distribution.

It does not publish the Portal, private Core, private implementation or a
current installable DUBSAR component.

No current public software licence is selected or granted by this repository.
Future component licensing remains deferred. The exact historical private-beta
licence remains with its tombstone and is not a current root licence.
Third-party licences remain unaffected. See [RIGHTS.md](RIGHTS.md).

## Claim controls

The public documentation must not imply:

- general portal availability;
- production readiness from an API or interface proof;
- automatic causality or complete source coverage;
- AI Act certification or legal advice;
- availability of an installed DUBSAR product;
- a coding-agent beta or Marketplace package;
- that public skills contain or unlock private DUBSAR components.

## Canonical references

- [README](README.md)
- [Status](STATUS.md)
- [Product and surfaces](PRODUCT_SURFACES.md)
- [Architecture](ARCHITECTURE.md)
- [Audit method](AUDIT.md)
- [Roadmap](ROADMAP.md)
- [Installation](INSTALLATION.md)
- [Marketplace history](MARKETPLACE.md)
- [Rights and licensing status](RIGHTS.md)

## Canonical status

```text
public documentation alignment: review branch
automated audit portal: coming soon, not publicly available
professional DUBSAR Audit: available on request
public skills: separate MIT-licensed companion resource
historical coding-agent package: paused; no active beta
historical Marketplace surface: retired from active tree
supported public DUBSAR installation: none
private Core: not published
component licensing decisions: deferred
general production availability: not claimed
```

</details>
