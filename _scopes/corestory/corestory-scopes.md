---
api_specs:
- filename: corestory-openapi-original.json
  format: json
  label: CoreStory API
  slug: corestory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corestory/refs/heads/main/openapi/corestory-openapi-original.json
authorization_urls:
- https://clerk.corestory.ai/oauth/authorize
description: ''
docs: https://docs.corestory.ai/getting-started/mcp-server-setup
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Corestory Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CoreStory publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CoreStory API on a user''s behalf.


  Tokens are issued from https://clerk.corestory.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CoreStory
provider_slug: corestory
schemes:
- flows:
  - authorizationUrl: https://clerk.corestory.ai/oauth/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    tokenUrl: https://clerk.corestory.ai/oauth/token
  name: OAuth2 (Clerk)
  source: https://clerk.corestory.ai/.well-known/oauth-authorization-server
scope_count: 7
scope_names:
- openid
- profile
- email
- public_metadata
- private_metadata
- offline_access
- user:org:read
scopes:
- description: OpenID Connect authentication.
  flows: []
  scope: openid
- description: Access the user's profile. Advertised by the MCP protected-resource metadata.
  flows: []
  scope: profile
- description: Access the user's email. Advertised by the MCP protected-resource metadata.
  flows: []
  scope: email
- description: Read the user's public metadata.
  flows: []
  scope: public_metadata
- description: Read the user's private metadata.
  flows: []
  scope: private_metadata
- description: Obtain a refresh token for offline access.
  flows: []
  scope: offline_access
- description: Read the user's organization membership.
  flows: []
  scope: user:org:read
slug: corestory-scopes
source_filename: corestory-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://c2s.corestory.ai/.well-known/oauth-protected-resource\ndocs: https://docs.corestory.ai/getting-started/mcp-server-setup\nschemes:\n- name: OAuth2 (Clerk)\n  source: https://clerk.corestory.ai/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clerk.corestory.ai/oauth/authorize\n    tokenUrl: https://clerk.corestory.ai/oauth/token\n    grant_types: [authorization_code, refresh_token]\nmcp_resource:\n  resource: https://c2s.corestory.ai/mcp\n  authorization_servers: [https://clerk.corestory.ai]\n  bearer_methods_supported: [header]\n  scopes_supported: [profile, email]\nscopes:\n- scope: openid\n  description: OpenID Connect authentication.\n  sources: [https://clerk.corestory.ai/.well-known/oauth-authorization-server]\n- scope: profile\n  description: Access the user's profile. Advertised by the MCP protected-resource metadata.\n  sources: [https://c2s.corestory.ai/.well-known/oauth-protected-resource]\n\
  - scope: email\n  description: Access the user's email. Advertised by the MCP protected-resource metadata.\n  sources: [https://c2s.corestory.ai/.well-known/oauth-protected-resource]\n- scope: public_metadata\n  description: Read the user's public metadata.\n  sources: [https://clerk.corestory.ai/.well-known/oauth-authorization-server]\n- scope: private_metadata\n  description: Read the user's private metadata.\n  sources: [https://clerk.corestory.ai/.well-known/oauth-authorization-server]\n- scope: offline_access\n  description: Obtain a refresh token for offline access.\n  sources: [https://clerk.corestory.ai/.well-known/oauth-authorization-server]\n- scope: \"user:org:read\"\n  description: Read the user's organization membership.\n  sources: [https://clerk.corestory.ai/.well-known/oauth-authorization-server]\nnotes: >-\n  The OpenAPI declares only http-bearer (JWT) global security, but CoreStory's MCP\n  server is an OAuth-protected resource (RFC 9728) whose authorization server is\n\
  \  Clerk (clerk.corestory.ai). Scopes captured verbatim from the live well-known\n  metadata. The MCP resource advertises profile+email; Clerk advertises the fuller\n  scope set.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corestory/refs/heads/main/scopes/corestory-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Ai
- Code Intelligence
- Legacy Modernization
- Developer Tools
- Code Analysis
- Documentation
- MCP
- Agentic
token_urls:
- https://clerk.corestory.ai/oauth/token
---
