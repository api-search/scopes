---
authorization_urls:
- https://app.airops.com/oauth/authorize
description: ''
docs: https://docs.airops.com/mcp/mcp-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Airops Scopes
name_suffix: OAuth Scopes
note: Scopes are enumerated from the live OAuth 2.0 / OpenID Connect discovery documents published by AirOps. The OIDC discovery advertises openid/profile/ email/api; the OAuth authorization-server metadata advertises the single "api" scope used to authorize the hosted MCP server and API access. AirOps does not publish a granular per-resource scope taxonomy; the REST API is authorized with a workspace-scoped API key rather than fine-grained OAuth scopes.
overview: 'AirOps publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AirOps API on a user''s behalf.


  Tokens are issued from https://app.airops.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AirOps
provider_slug: airops
schemes:
- flows:
  - authorizationUrl: https://app.airops.com/oauth/authorize
    flow: authorizationCode
    pkce:
    - S256
    tokenUrl: https://app.airops.com/oauth/token
  name: oauth2
  source: https://app.airops.com/.well-known/oauth-authorization-server
scope_count: 4
scope_names:
- api
- openid
- profile
- email
scopes:
- description: Access the AirOps API and workspace resources on behalf of the user.
  flows:
  - authorizationCode
  scope: api
- description: OpenID Connect authentication (subject identity).
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the user's email claim.
  flows:
  - authorizationCode
  scope: email
slug: airops-scopes
source_filename: airops-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://app.airops.com/.well-known/openid-configuration\ndocs: https://docs.airops.com/mcp/mcp-server\nnote: >-\n  Scopes are enumerated from the live OAuth 2.0 / OpenID Connect discovery\n  documents published by AirOps. The OIDC discovery advertises openid/profile/\n  email/api; the OAuth authorization-server metadata advertises the single \"api\"\n  scope used to authorize the hosted MCP server and API access. AirOps does not\n  publish a granular per-resource scope taxonomy; the REST API is authorized with\n  a workspace-scoped API key rather than fine-grained OAuth scopes.\nschemes:\n- name: oauth2\n  source: https://app.airops.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.airops.com/oauth/authorize\n    tokenUrl: https://app.airops.com/oauth/token\n    pkce: [S256]\nscopes:\n- scope: api\n  description: Access the AirOps API and workspace resources\
  \ on behalf of the user.\n  flows: [authorizationCode]\n  sources: [well-known/airops-oauth-authorization-server.json]\n- scope: openid\n  description: OpenID Connect authentication (subject identity).\n  flows: [authorizationCode]\n  sources: [well-known/airops-openid-configuration.json]\n- scope: profile\n  description: Access to the user's basic profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/airops-openid-configuration.json]\n- scope: email\n  description: Access to the user's email claim.\n  flows: [authorizationCode]\n  sources: [well-known/airops-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/scopes/airops-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Applications
- AI
- Content
- SEO
- AEO
- Answer Engine Optimization
- Generative Engine Optimization
- Workflows
- MCP
- Analytics
token_urls:
- https://app.airops.com/oauth/token
---
