---
api_specs:
- filename: mireye-ask-api-openapi.yml
  format: yaml
  label: Mireye Ask API
  slug: mireye-ask-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-ask-api-openapi.yml
- filename: mireye-ask-site-api-openapi.yml
  format: yaml
  label: Mireye Ask Site API
  slug: mireye-ask-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-ask-site-api-openapi.yml
- filename: mireye-auth-api-openapi.yml
  format: yaml
  label: Mireye Auth API
  slug: mireye-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-auth-api-openapi.yml
- filename: mireye-authorize-api-openapi.yml
  format: yaml
  label: Mireye Authorize API
  slug: mireye-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-authorize-api-openapi.yml
- filename: mireye-feature-requests-api-openapi.yml
  format: yaml
  label: Mireye Feature Requests API
  slug: mireye-feature-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-feature-requests-api-openapi.yml
- filename: mireye-fetch-api-openapi.yml
  format: yaml
  label: Mireye Fetch API
  slug: mireye-fetch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-fetch-api-openapi.yml
- filename: mireye-healthz-api-openapi.yml
  format: yaml
  label: Mireye Healthz API
  slug: mireye-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-healthz-api-openapi.yml
- filename: mireye-mcp-api-openapi.yml
  format: yaml
  label: Mireye Mcp API
  slug: mireye-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-mcp-api-openapi.yml
- filename: mireye-meta-api-openapi.yml
  format: yaml
  label: Mireye Meta API
  slug: mireye-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-meta-api-openapi.yml
- filename: mireye-oauth-api-openapi.yml
  format: yaml
  label: Mireye Oauth API
  slug: mireye-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-oauth-api-openapi.yml
- filename: mireye-readyz-api-openapi.yml
  format: yaml
  label: Mireye Readyz API
  slug: mireye-readyz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-readyz-api-openapi.yml
- filename: mireye-register-api-openapi.yml
  format: yaml
  label: Mireye Register API
  slug: mireye-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-register-api-openapi.yml
- filename: mireye-revoke-api-openapi.yml
  format: yaml
  label: Mireye Revoke API
  slug: mireye-revoke-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-revoke-api-openapi.yml
- filename: mireye-sites-api-openapi.yml
  format: yaml
  label: Mireye Sites API
  slug: mireye-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-sites-api-openapi.yml
- filename: mireye-token-api-openapi.yml
  format: yaml
  label: Mireye Token API
  slug: mireye-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-token-api-openapi.yml
- filename: mireye-users-api-openapi.yml
  format: yaml
  label: Mireye Users API
  slug: mireye-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-users-api-openapi.yml
- filename: mireye-well-known-api-openapi.yml
  format: yaml
  label: Mireye .well Known API
  slug: mireye-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/openapi/mireye-well-known-api-openapi.yml
authorization_urls:
- https://api.mireye.com/authorize
description: ''
docs: https://docs.mireye.ai/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Mireye Scopes
name_suffix: OAuth Scopes
note: Scopes captured from the RFC 8414 authorization-server metadata and the auth docs; the OpenAPI declares no oauth2 securitySchemes so nothing was derivable from the spec.
overview: 'Mireye publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mireye API on a user''s behalf.


  Tokens are issued from https://api.mireye.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mireye
provider_slug: mireye
schemes:
- flows:
  - authorizationUrl: https://api.mireye.com/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://api.mireye.com/token
  name: mcpOAuth
  source: https://api.mireye.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp:tools
scopes:
- description: Authorizes calls to Mireye's MCP tools (mireye_ask, mireye_fetch) via the hosted /mcp endpoint. Not valid for direct /v1/* HTTP API calls.
  flows:
  - authorizationCode
  scope: mcp:tools
slug: mireye-scopes
source_filename: mireye-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.mireye.com/.well-known/oauth-authorization-server\ndocs: https://docs.mireye.ai/authentication\nnote: >-\n  Scopes captured from the RFC 8414 authorization-server metadata and the auth docs; the\n  OpenAPI declares no oauth2 securitySchemes so nothing was derivable from the spec.\nschemes:\n- name: mcpOAuth\n  source: https://api.mireye.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.mireye.com/authorize\n    tokenUrl: https://api.mireye.com/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: mcp:tools\n  description: Authorizes calls to Mireye's MCP tools (mireye_ask, mireye_fetch) via the hosted /mcp endpoint. Not valid for direct /v1/* HTTP API calls.\n  flows: [authorizationCode]\n  sources: ['https://api.mireye.com/.well-known/oauth-authorization-server']\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mireye/refs/heads/main/scopes/mireye-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Geospatial
- Geographic Information System
- Location
- AI Agents
- Model Context Protocol
- Government Data
- Risk
- Insurance
- Data
token_urls:
- https://api.mireye.com/token
---
