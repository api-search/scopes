---
authorization_urls:
- https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Persado Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Persado publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Persado API on a user''s behalf.


  Tokens are issued from https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Persado
provider_slug: persado
schemes:
- flows:
  - authorizationUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/auth
    flow: authorizationCode
    tokenUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token
  name: PersadoMCPGatewayOAuth
  resource: https://api.persado.com/mcp
  source: https://api.persado.com/.well-known/oauth-authorization-server
scope_count: 3
scope_names:
- mcp:tools
- openid
- offline_access
scopes:
- description: Invoke tools exposed by the Persado MCP Gateway. This is Persado's own custom scope and is the single gate on the entire agent surface — a token without it cannot call tools/list or tools/call.
  flows:
  - authorizationCode
  scope: mcp:tools
- description: Standard OpenID Connect authentication; returns an ID token identifying the user.
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token so an agent session can outlive the access-token lifetime without re-prompting the user.
  flows:
  - authorizationCode
  scope: offline_access
slug: persado-scopes
source_filename: persado-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://api.persado.com/.well-known/oauth-authorization-server,\n  https://api.persado.com/.well-known/oauth-protected-resource,\n  https://myaccount.persado.com/realms/persado-portal/.well-known/openid-configuration\ndocs: null\nnotes: >-\n  No provider-published scope reference page exists — Persado has no developer\n  portal. Every scope below was read verbatim from a discovery document Persado\n  serves. Descriptions for the three MCP-gateway scopes are written by API\n  Evangelist from their standard meanings and the resource they gate; the scope\n  STRINGS are Persado's. Keycloak's stock built-in scopes are listed separately\n  and are not part of the agent-facing contract.\n\nschemes:\n- name: PersadoMCPGatewayOAuth\n  source: https://api.persado.com/.well-known/oauth-authorization-server\n  resource: https://api.persado.com/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/auth\n\
  \    tokenUrl: https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token\n\nscopes:\n- scope: mcp:tools\n  description: >-\n    Invoke tools exposed by the Persado MCP Gateway. This is Persado's own\n    custom scope and is the single gate on the entire agent surface — a token\n    without it cannot call tools/list or tools/call.\n  flows: [authorizationCode]\n  custom: true\n  sources:\n  - https://api.persado.com/.well-known/oauth-authorization-server\n  - https://api.persado.com/.well-known/oauth-protected-resource\n  - https://myaccount.persado.com/realms/persado-portal/.well-known/openid-configuration\n- scope: openid\n  description: Standard OpenID Connect authentication; returns an ID token identifying the user.\n  flows: [authorizationCode]\n  custom: false\n  sources:\n  - https://api.persado.com/.well-known/oauth-authorization-server\n  - https://api.persado.com/.well-known/oauth-protected-resource\n- scope: offline_access\n  description: >-\n    Issue\
  \ a refresh token so an agent session can outlive the access-token\n    lifetime without re-prompting the user.\n  flows: [authorizationCode]\n  custom: false\n  sources:\n  - https://api.persado.com/.well-known/oauth-authorization-server\n  - https://api.persado.com/.well-known/oauth-protected-resource\n\nrealm_scopes:\n  note: >-\n    Advertised by the underlying Keycloak realm (persado-portal) but NOT by the\n    MCP gateway's protected-resource metadata. These are stock Keycloak client\n    scopes, not a Persado product surface. Recorded for completeness only.\n  source: https://myaccount.persado.com/realms/persado-portal/.well-known/openid-configuration\n  scopes:\n  - acr\n  - address\n  - basic\n  - email\n  - microprofile-jwt\n  - organization\n  - phone\n  - profile\n  - roles\n  - service_account\n  - web-origins\n\nsummary:\n  agent_facing_scope_count: 3\n  custom_scope_count: 1\n  realm_scope_count: 11\n  granularity: >-\n    Coarse. A single mcp:tools scope gates every tool\
  \ on the gateway; there is\n    no per-tool or read-vs-write scope separation. An agent granted mcp:tools\n    can call anything the server exposes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/persado/refs/heads/main/scopes/persado-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Ai Apps
- Artificial Intelligence
- Generative AI
- Marketing
- Customer Engagement
- Content Generation
- Personalization
- Agents
- MCP
- Compliance
- Financial Services
token_urls:
- https://myaccount.persado.com/realms/persado-portal/protocol/openid-connect/token
---
