# DUBSAR Public Review Checklist

Use this checklist before merging a public-positioning change, announcing access or publishing an adapter.

## 1. Product identity

- [ ] DUBSAR is the only current public product brand.
- [ ] Portal audit is the primary customer-facing path.
- [ ] Automations and AI agents are the primary problem space.
- [ ] Historical SCRIBE names appear only as compatibility or legacy context.
- [ ] Claude Code, Codex and Cursor remain secondary developer-adapter experiments.

## 2. Product truth

- [ ] Deterministic fixture validation is distinguished from an API test.
- [ ] API evidence is distinguished from a browser user E2E.
- [ ] The complete portal journey is not described as proved until it is.
- [ ] Live connectors are not described as generally available.
- [ ] Continuous governance and the DUBSAR Node are described as roadmap capabilities.
- [ ] No external agency pilot is implied before internal acceptance.

## 3. Audit semantics

- [ ] The audit scope, sources and time window remain explicit.
- [ ] Findings remain linked to evidence.
- [ ] Missing evidence can produce `not evaluable`.
- [ ] Zero findings is not presented as compliance.
- [ ] Deterministic results, agent explanations and human decisions remain distinct.
- [ ] CTRL-303 language stays bounded to evidence found in connected sources.

## 4. Authority model

- [ ] Hermes roles are non-authoritative.
- [ ] The private Core remains the canonical authority boundary.
- [ ] Human review is attributable and bound to the displayed review state.
- [ ] Agents cannot approve their own work.
- [ ] An unavailable authority path never becomes a reassuring state.

## 5. AI Act and regulation

- [ ] DUBSAR is not described as a certification.
- [ ] No automatic legal verdict is claimed.
- [ ] No legal advice is implied.
- [ ] Regulatory relevance is limited to governance evidence and documentation support.

## 6. Portal, privacy and security

- [ ] Public portal availability matches the real access state.
- [ ] Authentication and tenant isolation have evidence before public access.
- [ ] Imports, retention, deletion, logs and subprocessors are documented.
- [ ] No connector credential, token or real client evidence is public.
- [ ] A monitored security contact exists before general availability.

## 7. Local Node and desktop

- [ ] The Node is not described as released before a supported package exists.
- [ ] Source credentials are intended to remain local.
- [ ] Node authority is restricted to its approved boundary.
- [ ] Desktop is presented as technical administration, not a complete separate product.
- [ ] Installation, update, rollback and removal are proved before support is claimed.

## 8. Developer adapters and Marketplace

- [ ] Historical Marketplace staging is visibly unsupported.
- [ ] No public installation command is active.
- [ ] No vendored runtime is promoted before licence and compatibility review.
- [ ] Generic or default session fallback is removed before publication.
- [ ] Package, plugin and repository licence metadata are reconciled.
- [ ] Final source pin and integrity material describe the exact released bytes.

## 9. Public/private boundary

- [ ] No private Core or Backend source is published.
- [ ] No internal deployment topology, prompt or policy is exposed.
- [ ] No secret, token, signing material or confidential proof is present.
- [ ] Third-party attribution and licences are complete for every distributed component.
- [ ] Public examples use synthetic data.

## 10. Repository operations

- [ ] Changes are reviewed through a branch and PR.
- [ ] No merge occurs without explicit human review.
- [ ] Repository metadata and topics match the approved positioning.
- [ ] Legacy public repositories are clearly named, archived or explained.
- [ ] Marketplace activation is a separate approval from documentation merge.

## Expected verdict for this realignment

```text
public documentation realignment: reviewable
deterministic fixture controls: internally validated
API audit path: internal evidence recorded
complete portal browser E2E: not yet proved
public portal availability: not announced
continuous governance / DUBSAR Node: roadmap
developer Marketplace: inactive
general availability: no
```
