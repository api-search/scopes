---
api_specs:
- filename: surfe-account-api-openapi.yml
  format: yaml
  label: Surfe Account API
  slug: surfe-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-account-api-openapi.yml
- filename: surfe-companies-api-openapi.yml
  format: yaml
  label: Surfe Companies API
  slug: surfe-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-companies-api-openapi.yml
- filename: surfe-people-api-openapi.yml
  format: yaml
  label: Surfe People API
  slug: surfe-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-people-api-openapi.yml
- filename: surfe-recommendations-api-openapi.yml
  format: yaml
  label: Surfe Recommendations API
  slug: surfe-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-recommendations-api-openapi.yml
authorization_urls:
- https://mcp.eu.surfe.com/authorize
description: 'Surfe''s only OAuth scope surface is its hosted MCP server. The REST API is a bearer API key with no scopes at all. The MCP authorization server advertises exactly ONE scope — `surfe` — so authorization is all-or-nothing: a token that can read credits can also spend them on enrichment. Per-tool consent is pushed to the MCP client ("Each tool''s permission is set in your client"), not to the token.'
docs: https://developers.surfe.com/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Surfe Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Surfe publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Surfe API on a user''s behalf.


  Tokens are issued from https://mcp.eu.surfe.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Surfe
provider_slug: surfe
schemes:
- flows:
  - authorizationUrl: https://mcp.eu.surfe.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://mcp.eu.surfe.com/token
  issuer: https://mcp.eu.surfe.com/
  name: surfeMcpOAuth
  source: well-known/surfe-oauth-authorization-server.json
  surface: mcp
scope_count: 1
scope_names:
- surfe
scopes:
- description: The single scope advertised in scopes_supported. Grants access to the Surfe MCP tool surface (people search/enrich, company search/enrich, credits). Surfe publishes no per-resource or read-vs-write scope split.
  flows:
  - authorizationCode
  scope: surfe
slug: surfe-scopes
source_filename: surfe-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.eu.surfe.com/.well-known/oauth-authorization-server\ndocs: https://developers.surfe.com/mcp\ndescription: >-\n  Surfe's only OAuth scope surface is its hosted MCP server. The REST API is a\n  bearer API key with no scopes at all. The MCP authorization server advertises\n  exactly ONE scope — `surfe` — so authorization is all-or-nothing: a token that\n  can read credits can also spend them on enrichment. Per-tool consent is pushed\n  to the MCP client (\"Each tool's permission is set in your client\"), not to the\n  token.\nschemes:\n- name: surfeMcpOAuth\n  surface: mcp\n  source: well-known/surfe-oauth-authorization-server.json\n  issuer: https://mcp.eu.surfe.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.eu.surfe.com/authorize\n    tokenUrl: https://mcp.eu.surfe.com/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: surfe\n  description: >-\n    The single scope advertised\
  \ in scopes_supported. Grants access to the Surfe\n    MCP tool surface (people search/enrich, company search/enrich, credits).\n    Surfe publishes no per-resource or read-vs-write scope split.\n  flows: [authorizationCode]\n  sources: [well-known/surfe-oauth-authorization-server.json]\nrest_api_scopes: []\nrest_api_note: >-\n  https://developers.surfe.com/api-key documents a single bearer API key with no\n  scope, permission or role model. Every endpoint accepts the same key.\ngaps:\n- >-\n  No read-only scope: an agent that only needs `GET /v2/credits` must be granted\n  the same token that can start credit-consuming enrichment jobs.\n- 'No resource-scoped tokens: people, companies and recommendations are not separable.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/scopes/surfe-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- B2B Data
- Contact Data
- Sales Intelligence
- Enrichment
- Lead Generation
- CRM
- Prospecting
token_urls:
- https://mcp.eu.surfe.com/token
---
