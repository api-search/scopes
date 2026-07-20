---
api_specs:
- filename: brandtrack-openapi-original.yml
  format: yaml
  label: Brandtrack API
  slug: brandtrack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/openapi/brandtrack-openapi-original.yml
authorization_urls:
- https://api.brandtrack.fm/oauth/authorize
description: ''
docs: https://api.brandtrack.fm/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Brandtrack Scopes
name_suffix: OAuth Scopes
note: Brandtrack's public REST API documents only x-customer-api-key (header) auth. The OAuth surface below was discovered via RFC 8414 authorization-server metadata at api.brandtrack.fm and is not yet documented in the human docs. It exposes a single "mcp" scope, indicating an OAuth-guarded MCP/agent access path distinct from the REST API key.
overview: 'Brandtrack publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Brandtrack API on a user''s behalf.


  Tokens are issued from https://api.brandtrack.fm/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Brandtrack
provider_slug: brandtrack
schemes:
- flows:
  - authorizationUrl: https://api.brandtrack.fm/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce: S256
    revocationUrl: https://api.brandtrack.fm/oauth/revoke
    tokenUrl: https://api.brandtrack.fm/oauth/token
  name: OAuth2
  source: https://api.brandtrack.fm/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the Brandtrack MCP / agent surface guarded by OAuth 2.0.
  flows:
  - authorizationCode
  scope: mcp
slug: brandtrack-scopes
source_filename: brandtrack-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api.brandtrack.fm/.well-known/oauth-authorization-server\ndocs: https://api.brandtrack.fm/.well-known/oauth-authorization-server\nnote: >-\n  Brandtrack's public REST API documents only x-customer-api-key (header) auth. The\n  OAuth surface below was discovered via RFC 8414 authorization-server metadata at\n  api.brandtrack.fm and is not yet documented in the human docs. It exposes a single\n  \"mcp\" scope, indicating an OAuth-guarded MCP/agent access path distinct from the\n  REST API key.\nschemes:\n- name: OAuth2\n  source: https://api.brandtrack.fm/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.brandtrack.fm/oauth/authorize\n    tokenUrl: https://api.brandtrack.fm/oauth/token\n    revocationUrl: https://api.brandtrack.fm/oauth/revoke\n    pkce: S256\n    grant_types: [authorization_code, refresh_token]\nscopes:\n- scope: mcp\n  description: Access\
  \ the Brandtrack MCP / agent surface guarded by OAuth 2.0.\n  flows: [authorizationCode]\n  sources: [https://api.brandtrack.fm/.well-known/oauth-authorization-server]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandtrack/refs/heads/main/scopes/brandtrack-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Music
- Background Music
- Audio
- Streaming
- Retail
- Hospitality
- In-Store Experience
- Media
- Sound
token_urls:
- https://api.brandtrack.fm/oauth/token
---
