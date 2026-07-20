---
api_specs:
- filename: flint-agent-tasks-openapi.yml
  format: yaml
  label: Flint Agent Tasks API
  slug: flint-agent-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flint/refs/heads/main/openapi/flint-agent-tasks-openapi.yml
authorization_urls:
- https://clerk.tryflint.com/oauth/authorize
description: ''
docs: https://clerk.tryflint.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Flint Scopes
name_suffix: OAuth Scopes
note: OAuth applies to Flint's hosted MCP server only (the REST Agent Tasks API uses a bearer API key with no scope surface). The MCP protected-resource metadata advertises openid + offline_access; the Clerk authorization server exposes the full standard Clerk OIDC scope set below.
overview: 'Flint publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flint API on a user''s behalf.


  Tokens are issued from https://clerk.tryflint.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flint
provider_slug: flint
schemes:
- flows:
  - authorizationUrl: https://clerk.tryflint.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clerk.tryflint.com/oauth/token
  name: mcpOAuth
  source: https://mcp.tryflint.com
scope_count: 7
scope_names:
- openid
- offline_access
- profile
- email
- public_metadata
- private_metadata
- user:org:read
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: Access the user's basic profile claims.
  flows: []
  scope: profile
- description: Access the user's email address.
  flows: []
  scope: email
- description: Read the user's public metadata.
  flows: []
  scope: public_metadata
- description: Read the user's private metadata.
  flows: []
  scope: private_metadata
- description: Read the user's organization membership.
  flows: []
  scope: user:org:read
slug: flint-scopes
source_filename: flint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://mcp.tryflint.com/.well-known/oauth-protected-resource\ndocs: https://clerk.tryflint.com/.well-known/oauth-authorization-server\nnote: >-\n  OAuth applies to Flint's hosted MCP server only (the REST Agent Tasks API uses\n  a bearer API key with no scope surface). The MCP protected-resource metadata\n  advertises openid + offline_access; the Clerk authorization server exposes the\n  full standard Clerk OIDC scope set below.\nschemes:\n  - name: mcpOAuth\n    source: https://mcp.tryflint.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://clerk.tryflint.com/oauth/authorize\n        tokenUrl: https://clerk.tryflint.com/oauth/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; issue an ID token.\n    advertised_by_resource: true\n  - scope: offline_access\n    description: Issue a refresh token for long-lived access.\n    advertised_by_resource: true\n  - scope:\
  \ profile\n    description: Access the user's basic profile claims.\n  - scope: email\n    description: Access the user's email address.\n  - scope: public_metadata\n    description: Read the user's public metadata.\n  - scope: private_metadata\n    description: Read the user's private metadata.\n  - scope: \"user:org:read\"\n    description: Read the user's organization membership.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flint/refs/heads/main/scopes/flint-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- AI
- Marketing
- Landing Pages
- Agents
- MCP
- Web
- Advertising
token_urls:
- https://clerk.tryflint.com/oauth/token
---
