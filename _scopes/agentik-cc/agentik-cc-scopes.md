---
api_specs:
- filename: agentik-cc-discover-api-openapi.yml
  format: yaml
  label: Agentik Discover API
  slug: agentik-cc-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-discover-api-openapi.yml
- filename: agentik-cc-oauth-api-openapi.yml
  format: yaml
  label: Agentik OAuth API
  slug: agentik-cc-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-oauth-api-openapi.yml
- filename: agentik-cc-run-api-openapi.yml
  format: yaml
  label: Agentik Run API
  slug: agentik-cc-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-run-api-openapi.yml
- filename: agentik-cc-wallet-api-openapi.yml
  format: yaml
  label: Agentik Wallet API
  slug: agentik-cc-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-wallet-api-openapi.yml
authorization_urls:
- https://api.agentik.cc/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Agentik Cc Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Agentik publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agentik API on a user''s behalf.


  Tokens are issued from https://api.agentik.cc/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agentik
provider_slug: agentik-cc
schemes:
- description: 'OAuth for MCP clients: PKCE S256, dynamic client registration or client ID metadata documents, refresh token rotation. With agent onboarding enabled, a verified account approves a dedicated execution key; otherwise the legacy authorization page accepts an existing workspace key. Tokens inherit the key policy.'
  flows:
  - authorizationUrl: https://api.agentik.cc/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.agentik.cc/oauth/token
  name: oauth
  source: openapi/agentik-cc-openapi.yml
scope_count: 1
scope_names:
- run
scopes:
- description: Discover, inspect and run tools, paid from the workspace balance within the key's caps
  flows:
  - authorizationCode
  scope: run
slug: agentik-cc-scopes
source_filename: agentik-cc-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/agentik-cc-openapi.yml\nschemes:\n- name: oauth\n  source: openapi/agentik-cc-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.agentik.cc/oauth/authorize\n    tokenUrl: https://api.agentik.cc/oauth/token\n  description: 'OAuth for MCP clients: PKCE S256, dynamic client registration or client ID metadata\n    documents, refresh token rotation. With agent onboarding enabled, a verified account approves\n    a dedicated execution key; otherwise the legacy authorization page accepts an existing workspace\n    key. Tokens inherit the key policy.'\nscopes:\n- scope: run\n  description: Discover, inspect and run tools, paid from the workspace balance within the key's\n    caps\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/agentik-cc-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/agentik-cc/scopes/agentik-cc-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Artificial Intelligence
- Automation
- Tools
- MCP
- Software-as-a-Service
token_bound: false
token_urls:
- https://api.agentik.cc/oauth/token
---
