---
authorization_urls:
- https://runrun.it/api/v1.0/oauth/authorize
description: ''
docs: https://runrun.it/api/documentation
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Nova Lima Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Nova Lima publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nova Lima API on a user''s behalf.


  Tokens are issued from https://runrun.it/api/v1.0/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nova Lima
provider_slug: nova-lima
schemes:
- flows:
  - authorizationUrl: https://runrun.it/api/v1.0/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    registrationUrl: https://runrun.it/mcp/oauth/register
    revocationUrl: https://runrun.it/api/v1.0/oauth/revoke
    tokenUrl: https://runrun.it/api/v1.0/oauth/token
    token_endpoint_auth_methods:
    - client_secret_basic
    - client_secret_post
    - none
  name: OAuth2
  source: https://runrun.it/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- all
scopes:
- description: Full access. The authorization server advertises a single coarse-grained scope ("all"); it does not publish a fine-grained scope taxonomy.
  flows:
  - authorizationCode
  scope: all
slug: nova-lima-scopes
source_filename: nova-lima-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://runrun.it/.well-known/oauth-authorization-server\ndocs: https://runrun.it/api/documentation\nschemes:\n  - name: OAuth2\n    source: https://runrun.it/.well-known/oauth-authorization-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://runrun.it/api/v1.0/oauth/authorize\n        tokenUrl: https://runrun.it/api/v1.0/oauth/token\n        revocationUrl: https://runrun.it/api/v1.0/oauth/revoke\n        registrationUrl: https://runrun.it/mcp/oauth/register\n        code_challenge_methods: [S256]\n        token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\nscopes:\n  - scope: all\n    description: Full access. The authorization server advertises a single coarse-grained scope (\"all\"); it does not publish a fine-grained scope taxonomy.\n    flows: [authorizationCode]\n    sources: [https://runrun.it/.well-known/oauth-authorization-server]\nnotes: >-\n  scopes_supported\
  \ in the OAuth 2.0 Authorization Server Metadata is [\"all\"].\n  This is the scope surface used by the hosted MCP server\n  (https://runrun.it/mcp), whose protected-resource metadata also advertises\n  scopes_supported: [\"all\"].\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nova-lima/refs/heads/main/scopes/nova-lima-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Project Management
- Task Management
- Work Management
- Productivity
- Time Tracking
- Team Collaboration
- SaaS
- Brazil
token_urls:
- https://runrun.it/api/v1.0/oauth/token
---
