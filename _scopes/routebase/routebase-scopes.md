---
api_specs:
- filename: openapi.json
  format: json
  label: Routebase API
  slug: routebase-api
  spec_type: OpenAPI
  url: https://docs.routebase.dev/api/routebase-public-api/openapi.json
authorization_urls: []
description: ''
docs: https://docs.routebase.dev/api-keys/
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Routebase Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Routebase uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Routebase
provider_slug: routebase
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: routebase-scopes
source_filename: routebase-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-11'\nmethod: searched\nsource: |-\n  https://mcp.routebase.dev/.well-known/oauth-protected-resource and\n  https://api.routebase.dev/.well-known/oauth-protected-resource (identical\n  scopes_supported list), corroborated by https://docs.routebase.dev/api-keys/\n  which documents the same scope strings as API-key permissions.\ndocs: https://docs.routebase.dev/api-keys/\nmodel: |-\n  Scopes are the granular API-key/OAuth permissions, grouped by functional area and\n  formatted <area>:<action>. Keys default to full access or can be restricted to a\n  subset of scopes and projects. OIDC identity scopes (openid, profile, email, ...)\n  are served separately by the auth server metadata.\nauthorization_server: https://auth.routebase.dev/\nresource_scopes:\n- scope: projects:read\n- scope: projects:write\n- scope: projects:delete\n- scope: projects:manage-members\n- scope: specs:read\n- scope: specs:write\n- scope: specs:publish\n- scope: specs:delete\n- scope:\
  \ specs:branch\n- scope: specs:merge\n- scope: specs:review\n- scope: tests:read\n- scope: tests:write\n- scope: tests:execute\n- scope: security:read\n- scope: security:write\n- scope: security:execute\n- scope: mock-server:read\n- scope: mock-server:manage\n- scope: monitoring:read\n- scope: monitoring:write\n- scope: gateway:read\n- scope: gateway:write\n- scope: gateway:deploy\n- scope: catalog:read\n- scope: catalog:write\n- scope: docs:read\n- scope: docs:write\n- scope: docs:publish\n- scope: docs:manage-portal\n- scope: notifications:read\n- scope: notifications:manage\n- scope: ai:use\n- scope: ai:manage\n- scope: billing:read\n- scope: billing:manage\n- scope: org:manage-members\n- scope: org:manage-teams\n- scope: org:manage-settings\n- scope: org:manage-security\n- scope: org:manage-governance\n- scope: org:delete\noidc_scopes:\n  source: https://auth.routebase.dev/.well-known/openid-configuration\n  scopes_supported: [openid, profile, offline_access, name, given_name, family_name,\
  \ nickname, email, email_verified, picture, created_at, identities, phone, address]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routebase/refs/heads/main/scopes/routebase-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API lifecycle management
- API design
- OpenAPI
- API documentation
- API testing
- API mocking
- API monitoring
- API security
- MCP
- AI agents
- developer tools
- CI/CD
- REST
- OAuth 2.1
- SCIM
- Streamable HTTP
token_urls: []
---
