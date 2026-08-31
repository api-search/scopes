---
api_specs:
- filename: sybilion-alerts-api-openapi.yml
  format: yaml
  label: Sybilion Alerts API
  slug: sybilion-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-alerts-api-openapi.yml
- filename: sybilion-categories-api-openapi.yml
  format: yaml
  label: Sybilion Categories API
  slug: sybilion-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-categories-api-openapi.yml
- filename: sybilion-drivers-api-openapi.yml
  format: yaml
  label: Sybilion Drivers API
  slug: sybilion-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-drivers-api-openapi.yml
- filename: sybilion-forecasts-api-openapi.yml
  format: yaml
  label: Sybilion Forecasts API
  slug: sybilion-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-forecasts-api-openapi.yml
- filename: sybilion-health-api-openapi.yml
  format: yaml
  label: Sybilion Health API
  slug: sybilion-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-health-api-openapi.yml
- filename: sybilion-jobs-api-openapi.yml
  format: yaml
  label: Sybilion Jobs API
  slug: sybilion-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-jobs-api-openapi.yml
- filename: sybilion-me-api-openapi.yml
  format: yaml
  label: Sybilion Me API
  slug: sybilion-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-me-api-openapi.yml
- filename: sybilion-regions-api-openapi.yml
  format: yaml
  label: Sybilion Regions API
  slug: sybilion-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-regions-api-openapi.yml
- filename: sybilion-usage-api-openapi.yml
  format: yaml
  label: Sybilion Usage API
  slug: sybilion-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-usage-api-openapi.yml
authorization_urls:
- https://mcp.sybilion.dev/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Sybilion Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no oauth2 security scheme — the REST API is bearer-key only, and derive-oauth-scopes.py correctly found zero. The OAuth surface belongs entirely to the MCP server, and its scopes were read from the live RFC 8414 authorization-server metadata document, not from the docs (the docs never name a scope at all). These are the four standard OIDC/OAuth scopes; there are NO Sybilion-specific resource scopes, so the token is not least-privilege — an approved MCP client can reach every tool the connector exposes, including the two billed write tools (submit_forecast, get_alerts). Consent is per-connection, not per-capability.
overview: 'Sybilion publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sybilion API on a user''s behalf.


  Tokens are issued from https://mcp.sybilion.dev/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sybilion
provider_slug: sybilion
schemes:
- applies_to: https://mcp.sybilion.dev/mcp
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mcp.sybilion.dev/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    refreshUrl: https://mcp.sybilion.dev/oauth/token
    tokenUrl: https://mcp.sybilion.dev/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.sybilion.dev
  jwks_uri: https://sybilion.eu.auth0.com/.well-known/jwks.json
  name: mcp-oauth
  registration_endpoint: https://mcp.sybilion.dev/oauth/register
  revocation_endpoint: https://mcp.sybilion.dev/oauth/revoke
  source: https://mcp.sybilion.dev/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Standard OIDC scope requesting an ID token for the approving user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope for basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC scope for the approving user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Standard OAuth scope requesting a refresh token so the MCP client can keep calling after the access token expires without a second browser approval.
  flows:
  - authorizationCode
  scope: offline_access
slug: sybilion-scopes
source_filename: sybilion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://mcp.sybilion.dev/.well-known/oauth-authorization-server\nnote: >-\n  The OpenAPI declares no oauth2 security scheme — the REST API is bearer-key only, and\n  derive-oauth-scopes.py correctly found zero. The OAuth surface belongs entirely to the MCP server,\n  and its scopes were read from the live RFC 8414 authorization-server metadata document, not from\n  the docs (the docs never name a scope at all). These are the four standard OIDC/OAuth scopes; there\n  are NO Sybilion-specific resource scopes, so the token is not least-privilege — an approved MCP\n  client can reach every tool the connector exposes, including the two billed write tools\n  (submit_forecast, get_alerts). Consent is per-connection, not per-capability.\ndocs: null\nsurface: mcp\nschemes:\n  - name: mcp-oauth\n    type: oauth2\n    applies_to: https://mcp.sybilion.dev/mcp\n    source: https://mcp.sybilion.dev/.well-known/oauth-authorization-server\n\
  \    issuer: https://mcp.sybilion.dev\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.sybilion.dev/oauth/authorize\n        tokenUrl: https://mcp.sybilion.dev/oauth/token\n        refreshUrl: https://mcp.sybilion.dev/oauth/token\n        pkce: [S256, plain]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none, client_secret_post]\n    revocation_endpoint: https://mcp.sybilion.dev/oauth/revoke\n    registration_endpoint: https://mcp.sybilion.dev/oauth/register\n    dynamic_client_registration: true\n    jwks_uri: https://sybilion.eu.auth0.com/.well-known/jwks.json\nscopes:\n  - scope: openid\n    description: Standard OIDC scope requesting an ID token for the approving user.\n    flows: [authorizationCode]\n    sources: ['https://mcp.sybilion.dev/.well-known/oauth-authorization-server']\n    resource_specific: false\n  - scope: profile\n    description: Standard OIDC scope for basic profile claims.\n    flows:\
  \ [authorizationCode]\n    sources: ['https://mcp.sybilion.dev/.well-known/oauth-authorization-server']\n    resource_specific: false\n  - scope: email\n    description: Standard OIDC scope for the approving user's email address.\n    flows: [authorizationCode]\n    sources: ['https://mcp.sybilion.dev/.well-known/oauth-authorization-server']\n    resource_specific: false\n  - scope: offline_access\n    description: >-\n      Standard OAuth scope requesting a refresh token so the MCP client can keep calling after the\n      access token expires without a second browser approval.\n    flows: [authorizationCode]\n    sources: ['https://mcp.sybilion.dev/.well-known/oauth-authorization-server']\n    resource_specific: false\nsummary:\n  scopes_total: 4\n  resource_scopes: 0\n  identity_scopes: 4\n  least_privilege: false\n  rest_api_uses_oauth: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/scopes/sybilion-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Industrial market intelligence
- Commodity price forecasting
- Economic forecasting
- Time-series forecasting
- Procurement
- Supply-chain risk
- Trading analytics
- AI decision support
- MCP
- Agent-native
- Causal inference
- Anomaly detection
token_urls:
- https://mcp.sybilion.dev/oauth/token
---
