---
api_specs:
- filename: jasper-api-openapi.yml
  format: yaml
  label: Jasper API
  slug: jasper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/openapi/jasper-api-openapi.yml
authorization_urls:
- https://api.jasper.ai/oauth2/authorize
description: ''
docs: https://developers.jasper.ai/docs/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Jasper Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Jasper publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Jasper API on a user''s behalf.


  Tokens are issued from https://api.jasper.ai/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Jasper
provider_slug: jasper
schemes:
- flows:
  - authorizationUrl: https://api.jasper.ai/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.jasper.ai/oauth2/token
  name: OAuth2
  source: https://api.jasper.ai/.well-known/oauth-authorization-server
scope_count: 6
scope_names:
- mcp
- user
- user:read
- openid
- email
- profile
scopes:
- description: Access the Jasper hosted MCP server tools (brand voices, audiences, agents, content generation).
  flows:
  - authorizationCode
  scope: mcp
- description: Act on behalf of the authenticated Jasper user (default user scope for API/agent access).
  flows:
  - authorizationCode
  scope: user
- description: Read the authenticated user's Jasper profile and workspace membership.
  flows:
  - authorizationCode
  scope: user:read
- description: OpenID Connect authentication — issue an ID token for the user.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: jasper-scopes
source_filename: jasper-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://api.jasper.ai/.well-known/openid-configuration ;\n  https://api.jasper.ai/.well-known/oauth-authorization-server ;\n  https://mcp.jasper.ai/.well-known/oauth-protected-resource ;\n  openapi/jasper-api-openapi.yml\ndocs: https://developers.jasper.ai/docs/authentication\nspec_divergence: >-\n  The captured OpenAPI's oauth2 securityScheme declares only two scopes — `user:read` (\"Read user\n  information\") and `user` (\"Read and write user information\") — and every one of the 50 operations\n  requires `user`. The live RFC 8414 authorization-server document additionally advertises `mcp`,\n  `openid`, `email` and `profile`. The spec therefore under-declares the scope surface, and no\n  operation is scoped more finely than \"read and write user information\": there is no per-resource\n  authorization in the contract.\nschemes:\n- name: OAuth2\n  source: https://api.jasper.ai/.well-known/oauth-authorization-server\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.jasper.ai/oauth2/authorize\n    tokenUrl: https://api.jasper.ai/oauth2/token\nscopes:\n- scope: mcp\n  description: Access the Jasper hosted MCP server tools (brand voices, audiences, agents, content generation).\n  flows: [authorizationCode]\n- scope: user\n  description: Act on behalf of the authenticated Jasper user (default user scope for API/agent access).\n  flows: [authorizationCode]\n- scope: user:read\n  description: Read the authenticated user's Jasper profile and workspace membership.\n  flows: [authorizationCode]\n- scope: openid\n  description: OpenID Connect authentication — issue an ID token for the user.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the user's email address claim.\n  flows: [authorizationCode]\n- scope: profile\n  description: Access the user's basic profile claims.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/scopes/jasper-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Content Generation
- Marketing
- Generative AI
- Agents
- MCP
token_urls:
- https://api.jasper.ai/oauth2/token
---
