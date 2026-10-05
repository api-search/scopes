---
authorization_urls: []
description: Motadata ServiceOps issues OAuth 2.0 access tokens through a password grant at /api/oauth/token. The token response carries a `scope` field, but Motadata documents exactly one value and publishes no scopes/permissions reference page. Authorization is enforced by the ServiceOps user the token is minted for — the role and permission set of that account — rather than by scope. There is no consent screen and no scope selection step.
docs: https://docs.motadata.com/serviceops-docs/integration-docs/managing-request-using-api
flows:
- password
kind: oauth-scopes
layout: scope
method: searched
name: Motadata Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Motadata publishes 1 OAuth 2.0 scope via the password flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Motadata API on a user''s behalf.


  Tokens are issued from https://{serviceops-host}/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Motadata
provider_slug: motadata
schemes: []
scope_count: 1
scope_names:
- other-api-scope
scopes:
- description: The only scope value Motadata documents in the token response. It is not described as partitioning access to any subset of the API; it appears to be a constant.
  flows: []
  scope: other-api-scope
slug: motadata-scopes
source_filename: motadata-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Motadata\nproviderId: motadata\ngenerated: '2026-08-29'\nmethod: searched\nsource: https://docs.motadata.com/serviceops-docs/integration-docs/managing-request-using-api\ndocs: https://docs.motadata.com/serviceops-docs/integration-docs/managing-request-using-api\ndescription: >-\n  Motadata ServiceOps issues OAuth 2.0 access tokens through a password grant at\n  /api/oauth/token. The token response carries a `scope` field, but Motadata documents exactly\n  one value and publishes no scopes/permissions reference page. Authorization is enforced by the\n  ServiceOps user the token is minted for — the role and permission set of that account — rather\n  than by scope. There is no consent screen and no scope selection step.\napi: motadata:serviceops\nflows:\n  - flow: password\n    tokenUrl: https://{serviceops-host}/api/oauth/token\n    client_auth: 'Basic base64(ClientID:ClientSecret)'\nscopes:\n  -\
  \ name: other-api-scope\n    description: >-\n      The only scope value Motadata documents in the token response. It is not described as\n      partitioning access to any subset of the API; it appears to be a constant.\n    source: https://docs.motadata.com/serviceops-docs/integration-docs/managing-request-using-api\nscope_count: 1\nnotes:\n  - >-\n    ObserveOps (the other Motadata product) has no OAuth surface at all — it authenticates with a\n    Personal Access Token, a static cookie, or a username/password session, and authorizes by\n    user permissions. See authentication/motadata-authentication.yml.\n  - >-\n    No scopes were invented to fill this file. One documented scope is the honest count.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motadata/refs/heads/main/scopes/motadata-scopes.yml
summary_line: 1 scope · password
tags:
- AIOps
- Monitoring
- Observability
- ITSM
- Service Desk
- Network Monitoring
- Log Management
- IT Operations
- Application Performance Monitoring
- OpenTelemetry
token_bound: false
token_urls:
- https://{serviceops-host}/api/oauth/token
---
