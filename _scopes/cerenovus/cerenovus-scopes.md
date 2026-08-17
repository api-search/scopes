---
authorization_urls:
- https://api.cerenovus.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Cerenovus Scopes
name_suffix: OAuth Scopes
note: These nine scopes are published verbatim by Cerenovus in scopes_supported on BOTH its RFC 8414 authorization-server metadata and its RFC 9728 protected-resource metadata. Cerenovus publishes no scopes/permissions reference page, so no descriptions are recorded — the description fields below are deliberately null rather than invented. The scope names are the provider's; the meaning of each is not documented anywhere public and must not be guessed.
overview: 'Cerenovus publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cerenovus API on a user''s behalf.


  Tokens are issued from https://api.cerenovus.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cerenovus
provider_slug: cerenovus
schemes:
- flows:
  - authorizationUrl: https://api.cerenovus.ai/authorize
    flow: authorizationCode
    tokenUrl: https://api.cerenovus.ai/token
  name: CerenovusOAuth
  source: https://api.cerenovus.ai/.well-known/oauth-authorization-server
scope_count: 9
scope_names:
- vault:read
- vault:write
- dashboard:write
- mailbox:rw
- session:read
- session:control
- device:control
- agent:read
- agent:run
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: vault:read
- description: ''
  flows:
  - authorizationCode
  scope: vault:write
- description: ''
  flows:
  - authorizationCode
  scope: dashboard:write
- description: ''
  flows:
  - authorizationCode
  scope: mailbox:rw
- description: ''
  flows:
  - authorizationCode
  scope: session:read
- description: ''
  flows:
  - authorizationCode
  scope: session:control
- description: ''
  flows:
  - authorizationCode
  scope: device:control
- description: ''
  flows:
  - authorizationCode
  scope: agent:read
- description: ''
  flows:
  - authorizationCode
  scope: agent:run
slug: cerenovus-scopes
source_filename: cerenovus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://api.cerenovus.ai/.well-known/oauth-protected-resource\nnote: >-\n  These nine scopes are published verbatim by Cerenovus in scopes_supported on BOTH its\n  RFC 8414 authorization-server metadata and its RFC 9728 protected-resource metadata.\n  Cerenovus publishes no scopes/permissions reference page, so no descriptions are\n  recorded — the description fields below are deliberately null rather than invented.\n  The scope names are the provider's; the meaning of each is not documented anywhere\n  public and must not be guessed.\ndocs: null\ndocs_note: no public scopes or permissions reference page exists on cerenovus.ai\nschemes:\n- name: CerenovusOAuth\n  source: https://api.cerenovus.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.cerenovus.ai/authorize\n    tokenUrl: https://api.cerenovus.ai/token\nscope_count: 9\nscopes:\n- scope: vault:read\n  description:\
  \ null\n  flows:\n  - authorizationCode\n- scope: vault:write\n  description: null\n  flows:\n  - authorizationCode\n- scope: dashboard:write\n  description: null\n  flows:\n  - authorizationCode\n- scope: mailbox:rw\n  description: null\n  flows:\n  - authorizationCode\n- scope: session:read\n  description: null\n  flows:\n  - authorizationCode\n- scope: session:control\n  description: null\n  flows:\n  - authorizationCode\n- scope: device:control\n  description: null\n  flows:\n  - authorizationCode\n- scope: agent:read\n  description: null\n  flows:\n  - authorizationCode\n- scope: agent:run\n  description: null\n  flows:\n  - authorizationCode\nx-evidence:\n  fetched: '2026-08-14'\n  url: https://api.cerenovus.ai/.well-known/oauth-protected-resource\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cerenovus/refs/heads/main/scopes/cerenovus-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Company
- Artificial Intelligence
- AI Agents
- Enterprise Software
- Decision Intelligence
- Knowledge Management
- Private Equity
- Due Diligence
- Model Context Protocol
- Y Combinator
token_urls:
- https://api.cerenovus.ai/token
---
