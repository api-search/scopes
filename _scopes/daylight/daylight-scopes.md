---
authorization_urls: []
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Daylight Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Daylight publishes 2 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Daylight API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Daylight
provider_slug: daylight
schemes:
- applies_to: https://api.daylight.ai
  authorizationUrl: https://auth.app.daylight.ai/oauth2/v1/apps/authorize
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  issuer: https://auth.app.daylight.ai/v1/apps/Peuc12rtvwjSr4gXbIvmOHyv8UyFi29b
  name: daylight-api-oidc
  tokenUrl: https://auth.app.daylight.ai/oauth2/v1/apps/token
- applies_to: https://docs.daylight.ai/mcp
  authorizationUrl: https://docs.daylight.ai/mcp/oauth/authorize
  flows:
  - authorizationCode
  - clientCredentials
  - refreshToken
  issuer: https://docs.daylight.ai/mcp/oauth
  name: daylight-docs-mcp-oauth
  tokenUrl: https://docs.daylight.ai/mcp/oauth/token
scope_count: 2
scope_names:
- openid
- mcp:search
scopes:
- description: OpenID Connect authentication scope for the Daylight product API (api.daylight.ai).
  flows: []
  scope: openid
- description: Search access to the Daylight documentation MCP server (docs.daylight.ai/mcp).
  flows: []
  scope: mcp:search
slug: daylight-scopes
source_filename: daylight-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://api.daylight.ai/.well-known/oauth-protected-resource +\n  https://auth.app.daylight.ai/.../.well-known/openid-configuration +\n  https://docs.daylight.ai/.well-known/oauth-authorization-server\nschemes:\n- name: daylight-api-oidc\n  applies_to: https://api.daylight.ai\n  issuer: https://auth.app.daylight.ai/v1/apps/Peuc12rtvwjSr4gXbIvmOHyv8UyFi29b\n  authorizationUrl: https://auth.app.daylight.ai/oauth2/v1/apps/authorize\n  tokenUrl: https://auth.app.daylight.ai/oauth2/v1/apps/token\n  flows: [authorizationCode, clientCredentials, refreshToken]\n- name: daylight-docs-mcp-oauth\n  applies_to: https://docs.daylight.ai/mcp\n  issuer: https://docs.daylight.ai/mcp/oauth\n  authorizationUrl: https://docs.daylight.ai/mcp/oauth/authorize\n  tokenUrl: https://docs.daylight.ai/mcp/oauth/token\n  flows: [authorizationCode, clientCredentials, refreshToken]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication\
  \ scope for the Daylight product API (api.daylight.ai).\n  schemes: [daylight-api-oidc]\n- scope: mcp:search\n  description: Search access to the Daylight documentation MCP server (docs.daylight.ai/mcp).\n  schemes: [daylight-docs-mcp-oauth]\nnotes: >-\n  The product API advertises only the baseline `openid` scope in its published\n  protected-resource metadata; any finer-grained product scopes are not exposed\n  in public discovery (authenticated surface). No scope reference page is\n  published in the public docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daylight/refs/heads/main/scopes/daylight-scopes.yml
summary_line: 2 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- MDR
- Threat Detection
- Incident Response
- Agentic AI
- SOC
- MCP
token_urls: []
---
