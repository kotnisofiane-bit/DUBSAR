# Product and Surfaces

DUBSAR is one product with two successive operating modes:

1. **Audit** — understand a bounded automation perimeter, connect findings to evidence and obtain an explicit human decision.
2. **Governance** — when the audit proves the need, control sensitive agent or automation actions before execution.

The public product is **DUBSAR**. Users should not need to understand the historical SCRIBE names, internal repositories or individual infrastructure components.

---

## Product definition

DUBSAR is an evidence and authority layer for AI agents and business automations.

It is designed to work across tools rather than becoming dependent on a single workflow engine or coding-agent host.

```text
Authorized sources
  -> bounded evidence snapshot
  -> deterministic controls
  -> role-based analysis and explanation
  -> visible findings and limitations
  -> designated human decision
  -> report
  -> optional governed execution
```

The deterministic system and the agent system have different responsibilities. Agents can explore, correlate and explain. They cannot promote their own conclusion to canonical truth or approve their own action.

---

## 1. Public website

The website at `dubsar.ai` is the discovery and orientation surface.

Its role is to:

- explain the audit-first product;
- help a visitor understand whether the problem is relevant;
- show the method, trust boundaries and current limitations;
- direct the visitor to the controlled portal when access is available;
- offer optional human assistance after an initial result, not require it before every audit.

The website is not the audit engine and must not imply that a visual demonstration proves a working product.

---

## 2. DUBSAR Portal

The controlled DUBSAR Portal is the intended primary user workspace. Its public
hostname must not be advertised until the access, privacy and isolation
boundaries have passed review.

It is designed for business owners, automation leads, reviewers and other authorized users to:

- define the audit perimeter and authorized sources;
- start and follow a bounded audit;
- inspect findings, supporting evidence and limitations;
- classify a finding as confirmed, rejected, uncertain or accepted risk;
- identify the person responsible for the decision;
- obtain a stable report and evidence register;
- later view governed agents and automation activity when continuous governance is deployed.

The Portal is based on LibreChat as an interaction surface, but LibreChat is not the DUBSAR authority layer. Its own agents, conversations or interface state cannot replace Core decisions.

Current status: authentication has been observed and an API-level audit path has been exercised. The complete browser journey remains an internal acceptance target.

---

## 3. Evidence intake and connectors

An audit begins from an explicitly authorized and bounded evidence perimeter.

The first automation-coherence path uses n8n-style workflow and execution evidence together with a business source such as a CRM. Initial validation may use controlled exports or synthetic fixtures before live connectors are enabled.

Connector responsibilities include:

- declaring the source, account or workspace in scope;
- collecting only the fields required by the active audit;
- recording time window, version, truncation and availability;
- producing stable evidence references and digests;
- making partial, missing or unavailable coverage visible;
- remaining read-only by default.

A connector is replaceable infrastructure. It does not own DUBSAR rules, findings, Human Gates or canonical decisions.

HTTP or API integrations may be added progressively. A third-party product update must degrade into an explicit connector limitation, not an invented clean result.

---

## 4. Hermes orchestration and agent roles

Hermes provides the role-based agent runtime used by DUBSAR.

Depending on the audit, roles may help:

- inspect a bounded evidence set;
- identify candidate contradictions;
- cross-check observations;
- explain a deterministic control result;
- prepare a review packet or report section.

Agent roles remain non-authoritative:

- they cannot declare their own output verified;
- they cannot conceal missing evidence;
- they cannot turn an inference into an observed fact;
- they cannot approve a sensitive action;
- they cannot replace the deterministic evaluator.

The orchestration layer should keep role identity, inputs, outputs and evidence snapshot identity attributable.

---

## 5. Protected Backend

The Backend is the private service boundary between public or local surfaces and canonical DUBSAR state.

Its responsibilities include:

- authentication and authorization checks;
- request validation and rate boundaries;
- stable audit and run identity;
- evidence freezing and digest verification;
- controlled orchestration calls;
- rejection of stale, duplicate or incomplete protected mutations;
- explicit unavailable or partial states;
- bounded report and Human Gate APIs.

The Backend is not distributed through this public repository.

---

## 6. Private deterministic Core

The private Core is the authority and policy engine of DUBSAR.

It is intended to own canonical state for:

- audit scope and evidence snapshot identity;
- deterministic rule packs and their versions;
- findings, contradictions and evidence relationships;
- verification tiers and missing-evidence state;
- designated human decisions;
- Human Gates and single-use authorizations;
- policy decisions for future governed execution;
- replay, audit trail and reconciliation.

The Core remains proprietary and is not distributed here.

The Core does not make every business judgment automatically. It preserves deterministic boundaries, records what is known and routes protected judgment to the designated human authority.

---

## 7. Human Gate

The Human Gate is a product boundary, not a decorative confirmation button.

Before a protected conclusion or action:

- the reviewer must see the relevant findings, evidence and limitations;
- the displayed review state must have a stable identity;
- the decision must be attributable to an authorized person;
- the recorded decision must remain bound to that exact review state;
- technical or agent credentials must not impersonate the human decision;
- retry must not create multiple decisions or actions.

Human validation can confirm, correct, reject or accept a bounded risk. It cannot make missing evidence become verified evidence.

---

## 8. Report and evidence register

The audit output is a decision-ready report, not a generic agent conversation.

It should distinguish:

- observed facts;
- deterministic results;
- agent inferences or explanations;
- confirmed contradictions;
- missing or unavailable evidence;
- human decisions;
- residual risks and recommended next actions.

Every material finding should remain connected to stable evidence references and the rule-pack version used for the run.

---

## 9. DUBSAR Node and technical desktop

After an audit, some organizations may choose continuous governance.

The intended technical surface is a **DUBSAR Node** installed in or near the customer environment and managed through an administrator-facing desktop or dashboard.

Its later responsibilities may include:

- connecting approved local agents and automation systems;
- holding bounded runtime and connector configuration;
- requesting policy decisions before sensitive execution;
- enforcing `ALLOW`, `DENY`, `REQUIRE_HUMAN_APPROVAL` or bounded conditions;
- recording action, policy and decision evidence;
- exposing health, connector and queue state to the technical administrator.

This surface is not required for the first portal audit. Installation work and desktop prototypes exist, but no supported customer governance deployment is currently claimed.

The Node applies decisions. It does not become a second Core.

---

## 10. Developer-tool adapters

Claude Code, Codex and Cursor remain relevant integration environments.

They may later use thin adapters to:

- attach a development workspace to DUBSAR;
- preserve decisions and evidence across agent sessions;
- submit bounded actions for governance;
- display Human Gate state;
- support audits of agent-assisted development.

These adapters are experimental and are not the primary commercial entry point. DUBSAR should also be usable without requiring a customer to adopt a particular coding agent.

---

## 11. Optional accompanied audit

The portal journey is intended to remain useful without requiring Sofiane to manually conduct every initial audit.

Human assistance may be offered when a customer wants:

- a broader or unusual perimeter;
- interpretation of material findings;
- remediation prioritization;
- connector or DUBSAR Node installation;
- preparation for continuous governance.

This is an optional service around the product, not a mandatory bottleneck before every report.

---

## AI Act boundary

DUBSAR may help structure and preserve elements relevant to AI governance, including:

- inventories of systems, agents, owners and purposes;
- traceability of sources, versions, decisions and actions;
- documented human oversight;
- visible limitations and unavailable information.

DUBSAR does not provide legal advice, certify AI Act compliance or issue an automatic legal verdict. Regulatory texts can inform rule-pack design, but the product must keep legal interpretation and client responsibility explicit.

---

## Summary

```text
Website explains
Portal scopes, shows and records
Connectors collect bounded evidence
Hermes roles analyze and explain
Backend protects the boundary
Core evaluates and preserves authority
Human Gate assigns the decision
Report makes the result reviewable
Node applies approved governance later
```

**Agents propose. DUBSAR preserves and checks. Humans decide.**
