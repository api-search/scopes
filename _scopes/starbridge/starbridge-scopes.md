---
api_specs:
- filename: starbridge-bridges-api-openapi.yml
  format: yaml
  label: Starbridge Bridges API
  slug: starbridge-bridges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-bridges-api-openapi.yml
- filename: starbridge-buyer-api-openapi.yml
  format: yaml
  label: Starbridge Buyer API
  slug: starbridge-buyer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-buyer-api-openapi.yml
- filename: starbridge-columns-api-openapi.yml
  format: yaml
  label: Starbridge Columns API
  slug: starbridge-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-columns-api-openapi.yml
- filename: starbridge-external-mcp-api-openapi.yml
  format: yaml
  label: Starbridge External MCP API
  slug: starbridge-external-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-external-mcp-api-openapi.yml
- filename: starbridge-signal-api-openapi.yml
  format: yaml
  label: Starbridge Signal API
  slug: starbridge-signal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/openapi/starbridge-signal-api-openapi.yml
authorization_urls: []
description: ''
docs: https://hc.starbridge.ai/research/starbridge-mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Starbridge Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Starbridge uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Starbridge
provider_slug: starbridge
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: starbridge-scopes
source_filename: starbridge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://dashboard.starbridge.ai/.well-known/oauth-protected-resource (200) +\n  https://dashboard.starbridge.ai/.well-known/oauth-authorization-server (200)\ndocs: https://hc.starbridge.ai/research/starbridge-mcp\n# OAuth scopes are NOT declared in the OpenAPI: the REST API is protected by a\n# static HTTP Bearer API key with no securityScheme of type oauth2, so\n# derive-oauth-scopes.py finds zero. The scopes below are read verbatim from the\n# two RFC 8414 / RFC 9728 metadata documents Starbridge serves for its MCP surface,\n# saved in well-known/.\napplies_to:\n  surface: MCP (hosted OAuth server)\n  resource: https://dashboard.starbridge.ai/mcp/oauth\n  authorization_server: https://auth.starbridge.ai\n  rest_api: >-\n    Not scoped. The External Public API uses a single opaque Bearer API key issued at\n    https://dashboard.starbridge.ai/settings/api-keys; it carries no scope parameter.\nscope_count: 1\nscopes:\n-\
  \ name: mcp:tools\n  description: >-\n    Grants an MCP client the ability to list and call the Starbridge MCP tools for the\n    authenticated user's organization. This is the only resource scope Starbridge\n    advertises; data access is further constrained by the user's own territory and\n    permission assignments in the platform.\n  source: /.well-known/oauth-protected-resource (scopes_supported)\n  file: well-known/starbridge-oauth-protected-resource.json\nidentity_scopes:\n  note: >-\n    The authorization server is an Auth0 tenant and advertises the standard OIDC\n    identity scopes below. They authenticate the user; they do not grant Starbridge\n    data access.\n  source: /.well-known/oauth-authorization-server (scopes_supported)\n  file: well-known/starbridge-oauth-authorization-server.json\n  scopes:\n  - openid\n  - profile\n  - offline_access\n  - name\n  - given_name\n  - family_name\n  - nickname\n  - email\n  - email_verified\n  - picture\n  - created_at\n  - identities\n\
  \  - phone\n  - address\nflows:\n  authorization_code: true\n  pkce: true\n  pkce_methods: [S256, plain]\n  dynamic_client_registration: true\n  registration_endpoint: https://auth.starbridge.ai/oidc/register\n  refresh_token: true\n  device_code: true\n  bearer_methods_supported: [header]\nnotes: >-\n  Dynamic client registration plus PKCE means an MCP client can complete the flow\n  with no pre-provisioned credentials, which is why the plugin and custom-connector\n  install paths need only a URL. Scope granularity is coarse — a single mcp:tools\n  scope covers all eleven tools, including the one write tool (setBridgeRowStatus),\n  so a read-only MCP grant is not expressible.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starbridge/refs/heads/main/scopes/starbridge-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Artificial Intelligence
- Sales Intelligence
- Go-To-Market
- Public Sector
- Education
- Government
- Procurement
- Buyer Intelligence
- MCP
token_urls: []
---
