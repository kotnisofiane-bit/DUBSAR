# Security Policy

DUBSAR is under active development and is not generally available for production use.

## Supported versions

No public production version is currently supported.

Historical Marketplace or plugin staging files recoverable from Git history are
unsupported and must not be restored or installed in a production environment.

## Reporting a vulnerability

Until a dedicated monitored security channel is confirmed publicly, contact:

`contact@dubsar.ai`

Use `SECURITY` in the subject line and provide only the minimum information required to establish contact.

Do not include:

- credentials or tokens;
- private keys;
- cookies or session material;
- real client evidence;
- personal data;
- exploit code targeting a live third-party system;
- private Core material.

A secure exchange channel can be agreed after initial contact.

## Current public scope

Reports may concern:

- this public documentation repository;
- public marketing website behavior;
- unexpected exposure or access-control failure on a DUBSAR endpoint;
- authentication or authorization boundaries;
- accidental data or secret exposure;
- published adapter staging material.

Private repositories, client environments and third-party services must not be probed without explicit authorization.

## Product security model

DUBSAR is designed around:

- explicit identity;
- bounded evidence collection;
- least-privilege connectors;
- separation of browser, service, agent and human authority;
- deterministic state transitions;
- fail-closed behavior for protected operations;
- visible missing or unavailable evidence;
- private Core isolation;
- expurgated proof artifacts.

These are design requirements. They are not a claim that a public production security review has been completed.

## Portal boundary

The automated audit portal is coming soon. It remains under development and
validation and is not currently available for public use. Before any public
portal access is opened, DUBSAR must validate:

- registration and authentication;
- tenant and project isolation;
- upload and connector authorization;
- rate and abuse controls;
- secret handling;
- evidence retention and deletion;
- human-decision authentication;
- audit and administrative logging;
- backup and recovery;
- dependency and infrastructure review.

## Future local Node

The intended Node security model is:

- outbound authenticated HTTPS only;
- short-lived, scoped device authorization;
- source credentials retained locally;
- bounded and filtered evidence submission;
- no direct Node access to private Core writes or Human Gate authority.

No public Node package currently implements a supported production boundary.

## Disclosure status

A full vulnerability-disclosure and response SLA will be published before general availability.
