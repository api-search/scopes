---
api_specs:
- filename: deployxa-openapi-original.json
  format: json
  label: Deployxa Platform
  slug: deployxa-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deployxa/refs/heads/main/openapi/deployxa-openapi-original.json
authorization_urls:
- https://deployxa.com/login
- https://mcp.deployxa.com/oauth/authorize
description: ''
docs: https://deployxa.com/auth.md
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Deployxa Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no oauth2 securitySchemes; scopes are searched from the provider's live RFC 8414 authorization-server metadata. The primary-domain auth server advertises OIDC-style scopes; the MCP auth server advertises the resource scopes. No per-scope prose descriptions are published — names only.
overview: 'Deployxa publishes 11 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Deployxa API on a user''s behalf.


  Tokens are issued from https://deployxa.com/api/auth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Deployxa
provider_slug: deployxa
schemes:
- flows:
  - authorizationUrl: https://deployxa.com/login
    flow: authorizationCode
    tokenUrl: https://deployxa.com/api/auth/token
  name: Deployxa OAuth (deployxa.com)
  source: https://deployxa.com/.well-known/oauth-authorization-server
- flows:
  - authorizationUrl: https://mcp.deployxa.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mcp.deployxa.com/oauth/token
  name: Deployxa MCP OAuth (mcp.deployxa.com)
  source: https://mcp.deployxa.com/.well-known/oauth-authorization-server
scope_count: 11
scope_names:
- openid
- profile
- email
- projects:read
- projects:write
- deployments:read
- deployments:write
- domains:read
- domains:write
- logs:read
- billing:read
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: openid
- description: ''
  flows:
  - authorizationCode
  scope: profile
- description: ''
  flows:
  - authorizationCode
  scope: email
- description: ''
  flows:
  - authorizationCode
  scope: projects:read
- description: ''
  flows:
  - authorizationCode
  scope: projects:write
- description: ''
  flows:
  - authorizationCode
  scope: deployments:read
- description: ''
  flows:
  - authorizationCode
  scope: deployments:write
- description: ''
  flows:
  - authorizationCode
  scope: domains:read
- description: ''
  flows:
  - authorizationCode
  scope: domains:write
- description: ''
  flows:
  - authorizationCode
  scope: logs:read
- description: ''
  flows:
  - authorizationCode
  scope: billing:read
slug: deployxa-scopes
source_filename: deployxa-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: https://mcp.deployxa.com/.well-known/oauth-authorization-server\ndocs: https://deployxa.com/auth.md\nnote: >-\n  The OpenAPI declares no oauth2 securitySchemes; scopes are searched from the\n  provider's live RFC 8414 authorization-server metadata. The primary-domain\n  auth server advertises OIDC-style scopes; the MCP auth server advertises the\n  resource scopes. No per-scope prose descriptions are published — names only.\nschemes:\n  - name: Deployxa OAuth (deployxa.com)\n    source: https://deployxa.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://deployxa.com/login\n        tokenUrl: https://deployxa.com/api/auth/token\n  - name: Deployxa MCP OAuth (mcp.deployxa.com)\n    source: https://mcp.deployxa.com/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.deployxa.com/oauth/authorize\n\
  \        tokenUrl: https://mcp.deployxa.com/oauth/token\nscopes:\n  - scope: openid\n    flows: [authorizationCode]\n    sources: [https://deployxa.com/.well-known/oauth-authorization-server]\n  - scope: profile\n    flows: [authorizationCode]\n    sources: [https://deployxa.com/.well-known/oauth-authorization-server]\n  - scope: email\n    flows: [authorizationCode]\n    sources: [https://deployxa.com/.well-known/oauth-authorization-server]\n  - scope: projects:read\n    flows: [authorizationCode]\n    sources: [https://mcp.deployxa.com/.well-known/oauth-authorization-server]\n  - scope: projects:write\n    flows: [authorizationCode]\n    sources: [https://mcp.deployxa.com/.well-known/oauth-authorization-server]\n  - scope: deployments:read\n    flows: [authorizationCode]\n    sources: [https://mcp.deployxa.com/.well-known/oauth-authorization-server]\n  - scope: deployments:write\n    flows: [authorizationCode]\n    sources: [https://mcp.deployxa.com/.well-known/oauth-authorization-server]\n\
  \  - scope: domains:read\n    flows: [authorizationCode]\n    sources: [https://mcp.deployxa.com/.well-known/oauth-authorization-server]\n  - scope: domains:write\n    flows: [authorizationCode]\n    sources: [https://mcp.deployxa.com/.well-known/oauth-authorization-server]\n  - scope: logs:read\n    flows: [authorizationCode]\n    sources: [https://mcp.deployxa.com/.well-known/oauth-authorization-server]\n  - scope: billing:read\n    flows: [authorizationCode]\n    sources: [https://mcp.deployxa.com/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deployxa/refs/heads/main/scopes/deployxa-scopes.yml
summary_line: 11 scopes · authorizationCode
tags:
- platform-as-a-service
- cloud-deployment
- devops
- ci-cd
- containers-docker
- edge-hosting
- managed-databases
- ai-ops
- developer-tools
token_urls:
- https://deployxa.com/api/auth/token
- https://mcp.deployxa.com/oauth/token
---
