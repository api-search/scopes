---
api_specs:
- filename: shortcut-software-openapi-original.json
  format: json
  label: Shortcut API
  slug: shortcut-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shortcut-software/refs/heads/main/openapi/shortcut-software-openapi-original.json
authorization_urls:
- https://api.app.shortcut.com/oauth-authorization-code-flow/code
description: ''
docs: https://www.shortcut.com/release-notes/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Shortcut Software Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Shortcut Software publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Shortcut Software API on a user''s behalf.


  Tokens are issued from https://api.app.shortcut.com/oauth-authorization-code-flow/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Shortcut Software
provider_slug: shortcut-software
schemes:
- flows:
  - authorizationUrl: https://api.app.shortcut.com/oauth-authorization-code-flow/code
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.app.shortcut.com/oauth-client-registration-flow/register
    tokenUrl: https://api.app.shortcut.com/oauth-authorization-code-flow/token
  issuer: https://api.app.shortcut.com
  name: OAuth2
  source: well-known/shortcut-software-oauth-authorization-server.json
scope_count: 6
scope_names:
- openid
- read
- write
- story-write
- comment-write
- admin
scopes:
- description: OpenID Connect authentication of the Shortcut member.
  flows:
  - authorizationCode
  scope: openid
- description: Read-only access to workspace data.
  flows:
  - authorizationCode
  scope: read
- description: Read/write access to workspace data.
  flows:
  - authorizationCode
  scope: write
- description: Create and update Stories.
  flows:
  - authorizationCode
  scope: story-write
- description: Create and update comments.
  flows:
  - authorizationCode
  scope: comment-write
- description: Administrative access to the workspace.
  flows:
  - authorizationCode
  scope: admin
slug: shortcut-software-scopes
source_filename: shortcut-software-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.app.shortcut.com/.well-known/oauth-authorization-server\ndocs: https://www.shortcut.com/release-notes/\nschemes:\n- name: OAuth2\n  source: well-known/shortcut-software-oauth-authorization-server.json\n  issuer: https://api.app.shortcut.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.app.shortcut.com/oauth-authorization-code-flow/code\n    tokenUrl: https://api.app.shortcut.com/oauth-authorization-code-flow/token\n    registrationUrl: https://api.app.shortcut.com/oauth-client-registration-flow/register\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect authentication of the Shortcut member.\n  flows: [authorizationCode]\n- scope: read\n  description: Read-only access to workspace data.\n  flows: [authorizationCode]\n- scope: write\n  description: Read/write access to workspace data.\n  flows: [authorizationCode]\n- scope: story-write\n  description: Create and\
  \ update Stories.\n  flows: [authorizationCode]\n- scope: comment-write\n  description: Create and update comments.\n  flows: [authorizationCode]\n- scope: admin\n  description: Administrative access to the workspace.\n  flows: [authorizationCode]\nnotes: >-\n  OAuth 2.0 (authorization code + PKCE, dynamic client registration) is advertised\n  via the RFC 8414 metadata document and backs the hosted MCP server. The primary\n  REST auth remains the Shortcut-Token API key header. As of the 2026-01-20 release,\n  API tokens themselves also support read-only vs read/write scoped permissions.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shortcut-software/refs/heads/main/scopes/shortcut-software-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Company
- Project Management
- Issue Tracking
- Agile
- Developer Tools
- Software Development
- Sprints
- Roadmaps
token_urls:
- https://api.app.shortcut.com/oauth-authorization-code-flow/token
---
