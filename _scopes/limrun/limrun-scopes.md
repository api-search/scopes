---
api_specs:
- filename: limrun-openapi-original.yml
  format: yaml
  label: Limrun API
  slug: limrun-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/openapi/limrun-openapi-original.yml
authorization_urls:
- https://api.limrun.com/authn/oauth/authorize
description: ''
docs: https://docs.limrun.com/docs/agents/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Limrun Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Limrun publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Limrun API on a user''s behalf.


  Tokens are issued from https://api.limrun.com/authn/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Limrun
provider_slug: limrun
schemes:
- dynamic_client_registration: true
  flows:
  - authorizationUrl: https://api.limrun.com/authn/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://api.limrun.com/authn/oauth/token
  issuer: https://api.limrun.com
  name: MCPOAuth
  source: https://api.limrun.com/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access to Limrun's Model Context Protocol surface. Advertised as the sole entry of scopes_supported by the authorization-server metadata; the provider publishes no further description of what the scope grants.
  flows:
  - authorizationCode
  scope: mcp
slug: limrun-scopes
source_filename: limrun-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.limrun.com/.well-known/oauth-authorization-server\ndocs: https://docs.limrun.com/docs/agents/mcp\nnotes: >-\n  Limrun's primary API authentication is a bearer org API key, not OAuth, so there is no\n  general-purpose scope surface. The one OAuth surface is the authorization server advertised at\n  api.limrun.com for MCP clients, which publishes a single supported scope. Captured from the live\n  RFC 8414 document; the provider does not publish a prose scopes reference page.\nschemes:\n- name: MCPOAuth\n  source: https://api.limrun.com/.well-known/oauth-authorization-server\n  issuer: https://api.limrun.com\n  dynamic_client_registration: true\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.limrun.com/authn/oauth/authorize\n    tokenUrl: https://api.limrun.com/authn/oauth/token\n    code_challenge_methods:\n    - S256\nscopes:\n- scope: mcp\n  description: >-\n    Access to Limrun's Model\
  \ Context Protocol surface. Advertised as the sole entry of\n    scopes_supported by the authorization-server metadata; the provider publishes no further\n    description of what the scope grants.\n  flows:\n  - authorizationCode\n  sources:\n  - https://api.limrun.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/limrun/refs/heads/main/scopes/limrun-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Mobile
- iOS
- Android
- Simulators
- Emulators
- Cloud Infrastructure
- Continuous Integration
- Developer Tools
- Testing
- Agents
- Model Context Protocol
- Sandboxes
- Xcode
token_urls:
- https://api.limrun.com/authn/oauth/token
---
