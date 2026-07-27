---
api_specs:
- filename: yardi-canada-status-openapi.yml
  format: yaml
  label: Yardi Systems Status API
  slug: yardi-systems-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/openapi/yardi-canada-status-openapi.yml
authorization_urls:
- https://mcp.virtuoso.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Yardi Canada Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Yardi Canada publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Yardi Canada API on a user''s behalf.


  Tokens are issued from https://mcp.virtuoso.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Yardi Canada
provider_slug: yardi-canada
schemes:
- flows:
  - authorizationUrl: https://mcp.virtuoso.ai/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    registrationUrl: https://mcp.virtuoso.ai/oauth/register
    tokenUrl: https://mcp.virtuoso.ai/oauth/token
    token_endpoint_auth_methods:
    - client_secret_post
    - client_secret_basic
    - none
  issuer: https://mcp.virtuoso.ai
  name: virtuoso-mcp-oauth
  source: https://mcp.virtuoso.ai/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Standard OpenID Connect scope; requests an ID token for the signed-in Yardi user.
  flows:
  - authorizationCode
  scope: openid
- description: Standard OIDC scope for basic profile claims about the signed-in Yardi user.
  flows:
  - authorizationCode
  scope: profile
- description: Standard OIDC scope for the signed-in user's email claim.
  flows:
  - authorizationCode
  scope: email
- description: Requests a refresh token so the agent can keep operating without re-consent.
  flows:
  - authorizationCode
  scope: offline_access
slug: yardi-canada-scopes
source_filename: yardi-canada-scopes.yml
source_heading: OAuth Scopes
source_url: https://mcp.virtuoso.ai/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://mcp.virtuoso.ai/.well-known/oauth-authorization-server\nsources:\n  - https://mcp.virtuoso.ai/.well-known/oauth-authorization-server\n  - https://mcp.virtuoso.ai/.well-known/oauth-protected-resource\nsummary: >-\n  Yardi's only published OAuth scope vocabulary belongs to the Yardi Virtuoso MCP\n  server, and it is deliberately thin: four standard OIDC/OAuth scopes, no\n  product-domain scopes. That is the whole authorization story an agent can read\n  anonymously. Data authorization is not expressed as scopes at all — Yardi states\n  the connector \"authenticates through Yardi, so data access automatically follows\n  existing user permissions\", which means the Voyager/Breeze/RentCafe role of the\n  signed-in Yardi user is the real permission boundary. No scope reference page is\n  published; the metadata document is the reference.\nschemes:\n  - name: virtuoso-mcp-oauth\n    type: oauth2\n    source: https://mcp.virtuoso.ai/.well-known/oauth-authorization-server\n\
  \    issuer: https://mcp.virtuoso.ai\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.virtuoso.ai/oauth/authorize\n        tokenUrl: https://mcp.virtuoso.ai/oauth/token\n        registrationUrl: https://mcp.virtuoso.ai/oauth/register\n        pkce: [S256]\n        grant_types: [authorization_code, refresh_token]\n        token_endpoint_auth_methods: [client_secret_post, client_secret_basic, none]\nscopes:\n  - scope: openid\n    description: Standard OpenID Connect scope; requests an ID token for the signed-in Yardi user.\n    flows: [authorizationCode]\n    sources: [https://mcp.virtuoso.ai/.well-known/oauth-authorization-server]\n  - scope: profile\n    description: Standard OIDC scope for basic profile claims about the signed-in Yardi user.\n    flows: [authorizationCode]\n    sources: [https://mcp.virtuoso.ai/.well-known/oauth-authorization-server]\n  - scope: email\n    description: Standard OIDC scope for the signed-in user's email claim.\n    flows:\
  \ [authorizationCode]\n    sources: [https://mcp.virtuoso.ai/.well-known/oauth-authorization-server]\n  - scope: offline_access\n    description: Requests a refresh token so the agent can keep operating without re-consent.\n    flows: [authorizationCode]\n    sources: [https://mcp.virtuoso.ai/.well-known/oauth-authorization-server]\nnotes:\n  - No product-domain scopes (property, lease, ledger, work-order) are published; the connector is declared Read & Write with no scope-level separation of the two.\n  - No OAuth surface of any kind exists on www.yardi.com or www.yardibreeze.ca — /.well-known/openid-configuration and /.well-known/oauth-authorization-server both 404 there.\n  - The Voyager Standard Interfaces and the RentCafe API are not OAuth; they use a contract-issued access token (see authentication/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yardi-canada/refs/heads/main/scopes/yardi-canada-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Real Estate
- Canada
- Property Management
- Rentals
- Commercial Real Estate
- PropTech
- Multifamily
- Affordable Housing
- Senior Living
- Investment Management
- Tenancy
- Payments
- MCP
- AI
token_urls:
- https://mcp.virtuoso.ai/oauth/token
---
