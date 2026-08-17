---
authorization_urls:
- https://mcp.demostack.com/authorize
description: Demostack publishes no scopes reference page and no OpenAPI with oauth2 securitySchemes. The scopes below were read directly from the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata served by the Demostack MCP host — the only place Demostack publishes a scope list. They are the standard OpenID Connect / OAuth set; Demostack declares no product-specific scopes (no read:demos, write:tours, or similar), so an agent cannot request or reason about least-privilege access to Demostack data.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Demostack Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Demostack publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Demostack API on a user''s behalf.


  Tokens are issued from https://mcp.demostack.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Demostack
provider_slug: demostack
schemes:
- flows:
  - authorizationUrl: https://mcp.demostack.com/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.demostack.com/token
  name: demostack-mcp-oauth
  source: well-known/demostack-oauth-authorization-server.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: Request an OpenID Connect subject identifier for the authenticated user.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows:
  - authorizationCode
  scope: profile
- description: Email address claim for the authenticated user.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token so the client can act after the access token expires.
  flows:
  - authorizationCode
  scope: offline_access
slug: demostack-scopes
source_filename: demostack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.demostack.com/.well-known/oauth-authorization-server\ndescription: >-\n  Demostack publishes no scopes reference page and no OpenAPI with oauth2\n  securitySchemes. The scopes below were read directly from the RFC 8414\n  authorization-server metadata and the RFC 9728 protected-resource metadata\n  served by the Demostack MCP host — the only place Demostack publishes a scope\n  list. They are the standard OpenID Connect / OAuth set; Demostack declares no\n  product-specific scopes (no read:demos, write:tours, or similar), so an agent\n  cannot request or reason about least-privilege access to Demostack data.\n\nschemes:\n  - name: demostack-mcp-oauth\n    source: well-known/demostack-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.demostack.com/authorize\n        tokenUrl: https://mcp.demostack.com/token\n\nscopes:\n  - scope: openid\n    description:\
  \ Request an OpenID Connect subject identifier for the authenticated user.\n    flows: [authorizationCode]\n    sources:\n      - well-known/demostack-oauth-authorization-server.json\n      - well-known/demostack-oauth-protected-resource.json\n  - scope: profile\n    description: Basic profile claims for the authenticated user.\n    flows: [authorizationCode]\n    sources:\n      - well-known/demostack-oauth-authorization-server.json\n      - well-known/demostack-oauth-protected-resource.json\n  - scope: email\n    description: Email address claim for the authenticated user.\n    flows: [authorizationCode]\n    sources:\n      - well-known/demostack-oauth-authorization-server.json\n      - well-known/demostack-oauth-protected-resource.json\n  - scope: offline_access\n    description: Issue a refresh token so the client can act after the access token expires.\n    flows: [authorizationCode]\n    sources:\n      - well-known/demostack-oauth-authorization-server.json\n      - well-known/demostack-oauth-protected-resource.json\n\
  \nresource:\n  resource: https://mcp.demostack.com/mcp\n  authorization_servers:\n    - https://mcp.demostack.com/\n  scopes_supported: [openid, profile, email, offline_access]\n  bearer_methods_supported: [header]\n\nsummary:\n  scope_count: 4\n  product_scopes: 0\n  note: >-\n    All four scopes are identity scopes. Authorization to Demostack data is\n    decided server-side from the authenticated user's tenant and role, not from\n    a requested scope.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demostack/refs/heads/main/scopes/demostack-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Sales Demo
- Demo Automation
- Product Simulation
- Webhooks
- CRM Integration
- Sales Enablement
- Presales
- Sales Engineering
- Analytics
- AI
- MCP
token_urls:
- https://mcp.demostack.com/token
---
