---
api_specs:
- filename: fastdrop-dev-health-api-openapi.yml
  format: yaml
  label: FastDrop Health API
  slug: fastdrop-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-health-api-openapi.yml
- filename: fastdrop-dev-mcp-api-openapi.yml
  format: yaml
  label: FastDrop MCP API
  slug: fastdrop-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-mcp-api-openapi.yml
- filename: fastdrop-dev-subregistry-api-openapi.yml
  format: yaml
  label: FastDrop Subregistry API
  slug: fastdrop-dev-subregistry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastdrop-dev/openapi/fastdrop-dev-subregistry-api-openapi.yml
authorization_urls:
- https://fastdrop.dev/api/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Fastdrop Dev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FastDrop publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FastDrop API on a user''s behalf.


  Tokens are issued from https://fastdrop.dev/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FastDrop
provider_slug: fastdrop-dev
schemes:
- description: OAuth 2 for MCP clients (RFC 8414 metadata at /.well-known/oauth-authorization-server, protected-resource metadata at /.well-known/oauth-protected-resource/mcp). Public clients supported (empty client secret on the token endpoint).
  flows:
  - authorizationUrl: https://fastdrop.dev/api/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://fastdrop.dev/api/auth/oauth2/token
  name: FastDropOAuth
  source: openapi/fastdrop-dev-openapi.json
scope_count: 2
scope_names:
- mcp
- offline_access
scopes:
- description: Call the FastDrop MCP server (/mcp) on behalf of the signed-in user. Read tools plus their own submissions, votes, reviews, and comments - nothing else.
  flows:
  - authorizationCode
  scope: mcp
- description: Receive refresh tokens so a long-lived agent session can renew access without re-consent.
  flows:
  - authorizationCode
  scope: offline_access
slug: fastdrop-dev-scopes
source_filename: fastdrop-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fastdrop-dev-openapi.json\nschemes:\n- name: FastDropOAuth\n  source: openapi/fastdrop-dev-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fastdrop.dev/api/auth/oauth2/authorize\n    tokenUrl: https://fastdrop.dev/api/auth/oauth2/token\n  description: OAuth 2 for MCP clients (RFC 8414 metadata at /.well-known/oauth-authorization-server,\n    protected-resource metadata at /.well-known/oauth-protected-resource/mcp). Public clients\n    supported (empty client secret on the token endpoint).\nscopes:\n- scope: mcp\n  description: Call the FastDrop MCP server (/mcp) on behalf of the signed-in user. Read tools\n    plus their own submissions, votes, reviews, and comments - nothing else.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fastdrop-dev-openapi.json\n- scope: offline_access\n  description: Receive refresh tokens so a long-lived agent session can renew access without\n\
  \    re-consent.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fastdrop-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fastdrop-dev/scopes/fastdrop-dev-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- launch-board
- MCP
- AI-agents
- software-discovery
- free-service
token_bound: false
token_urls:
- https://fastdrop.dev/api/auth/oauth2/token
---
