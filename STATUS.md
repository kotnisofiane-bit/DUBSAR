# Status

Last reviewed: 29 July 2026.

DUBSAR is being realigned around a **portal-first product for auditing and governing AI agents and business automations**.

The intended progression is:

```text
bounded audit
  -> evidence-backed findings
  -> explicit human validation
  -> report
  -> optional continuous governance when the need is proven
```

The audit is the entry point. Continuous governance and orchestration are the later operating mode. Developer-tool integrations remain useful experiments, but they are no longer the primary commercial entry point.

---

## Current surface status

| Surface | Current status |
|---|---|
| Public website | Repositioning toward automation audit and governance |
| DUBSAR Portal | Controlled test surface; account creation and sign-in have been observed |
| Portal audit journey | An API-level internal path has been recorded with fixtures; the complete browser user journey is not yet proven |
| Automation-coherence rules | Deterministic evaluation works on bounded synthetic fixtures; canonical packaging and missing-evidence behavior still require closure |
| Hermes role orchestration | Earlier internal tests launched role-based agents; the current deployed end-to-end path must be revalidated |
| Human validation and report | Components and API behavior exist; the final review-to-report journey through the user interface remains to be proven |
| Private Backend and Core | Active engineering components under reconciliation and integration testing; not distributed here |
| DUBSAR Node / technical desktop | Prototype and installation work exist; no supported customer governance deployment is claimed |
| Claude Code, Codex and Cursor adapters | Experimental technical path; secondary to the portal-first product |
| External agency pilot | Not started and not authorized before internal end-to-end acceptance |

---

## What has been demonstrated internally

The following observations are useful engineering evidence:

- deterministic automation controls can identify the planted incoherences in bounded n8n and business-source fixtures;
- the same evaluator can return no detected finding on a bounded healthy fixture without turning that absence into a general compliance claim;
- the portal test deployment has accepted account creation and sign-in;
- an API-driven audit path has exercised project creation, fixture submission, processing, human resolution and report retrieval;
- earlier local tests demonstrated that several Hermes roles could be launched;
- a Windows desktop shell has been packaged, installed and opened.

These observations do **not** prove that the complete product works for an ordinary user. In particular, an API test is not a browser test, an interface is not a connected workflow, and a desktop that opens is not proof of an operational governance installation.

---

## What is not yet proven

DUBSAR does not currently claim proof of:

- a complete portal journey performed only through the user interface, from sign-in to a stable downloadable report;
- production-grade live connectors to n8n, CRM, email or other business systems;
- a deployed Hermes, Backend and Core chain that survives retry, restart and partial failure without duplicate or misleading state;
- a Human Gate bound to the exact findings and evidence displayed to the reviewer;
- continuous pre-action governance inside a customer environment;
- an independently usable DUBSAR Node or technical desktop;
- an external agency pilot;
- general availability, production readiness or a supported public installation;
- AI Act compliance, legal advice, certification or an automatic legal verdict.

Missing or unavailable evidence must remain visible. It must never be silently converted into a pass.

---

## Current acceptance target

The next product proof is an **internal portal end-to-end test** using synthetic, non-sensitive fixtures.

The test must demonstrate, without manual API substitution:

1. account access through the browser;
2. creation of a bounded audit;
3. submission or selection of authorized fixture sources;
4. one stable audit identity despite retry or double-click;
5. deterministic rule evaluation tied to a frozen evidence snapshot;
6. role-based agent contributions that remain non-authoritative;
7. all findings, evidence, limitations and missing sources visible before validation;
8. an explicit client-side human decision tied to the displayed review state;
9. a report that remains stable after reload;
10. proof artifacts sufficient to reproduce and audit the run.

No real agency pilot should begin before this internal journey passes and receives explicit human approval.

---

## Product and authority boundary

- The **Portal** is the user workspace for audit scope, results, validation and reports.
- **Hermes and its roles** help collect, analyze and explain. They do not create canonical truth or authorize their own actions.
- The protected **Backend** enforces the service boundary.
- The private deterministic **Core** owns canonical rules, evidence state and protected decisions.
- The **Human Gate** returns final business authority to the designated person.
- A future **DUBSAR Node** may apply approved policies inside the customer environment after the audit has established a justified need.

**Agents propose. DUBSAR preserves and checks. Humans decide.**

---

## Public availability

```text
portal-first product: internal validation
public self-service audit: not yet available as a supported service
external agency pilot: not started
continuous governance / DUBSAR Node: future validated stage
developer adapters: experimental
private Core: proprietary, not distributed
general availability: no
AI Act certification or legal verdict: no
```

Any stronger readiness statement requires reproducible evidence and an explicit Human GO.
