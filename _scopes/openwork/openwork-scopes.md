---
api_specs:
- filename: openwork-den-openapi.json
  format: json
  label: OpenWork Den API
  slug: den-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openwork/refs/heads/main/openapi/openwork-den-openapi.json
authorization_urls: []
description: ''
docs: https://openworklabs.com/docs/api-reference
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Openwork Scopes
name_suffix: OAuth Scopes
note: OAuth 2.0 scopes are advertised via authorization-server / OIDC discovery and gate the OpenWork MCP endpoint (protected resource https://api.openworklabs.com/mcp). The Den REST API itself authenticates with session bearer tokens and organization API keys rather than scoped OAuth tokens.
overview: 'Openwork uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Openwork
provider_slug: openwork
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: openwork-scopes
source_filename: openwork-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.openworklabs.com/.well-known/oauth-authorization-server\ndocs: https://openworklabs.com/docs/api-reference\nauthorization_server:\n  issuer: https://app.openworklabs.com/api/auth\n  authorization_endpoint: https://app.openworklabs.com/api/auth/oauth2/authorize\n  token_endpoint: https://app.openworklabs.com/api/auth/oauth2/token\n  registration_endpoint: https://app.openworklabs.com/api/auth/oauth2/register\n  introspection_endpoint: https://app.openworklabs.com/api/auth/oauth2/introspect\n  revocation_endpoint: https://app.openworklabs.com/api/auth/oauth2/revoke\n  jwks_uri: https://app.openworklabs.com/api/auth/jwks\nnote: >-\n  OAuth 2.0 scopes are advertised via authorization-server / OIDC discovery and\n  gate the OpenWork MCP endpoint (protected resource https://api.openworklabs.com/mcp).\n  The Den REST API itself authenticates with session bearer tokens and\n  organization API keys rather than scoped OAuth\
  \ tokens.\nscopes:\n- name: openid\n  description: OpenID Connect authentication; issue an ID token for the signed-in user.\n- name: profile\n  description: Access the user's basic profile claims.\n- name: email\n  description: Access the user's email address claim.\n- name: offline_access\n  description: Issue a refresh token for long-lived, offline agent access.\n- name: mcp:read\n  description: Read access to the OpenWork MCP endpoint (list tools / resources, read state).\n- name: mcp:write\n  description: Write access to the OpenWork MCP endpoint (invoke tools that mutate state).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openwork/refs/heads/main/scopes/openwork-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- AI Agents
- Open Source
- Desktop
- Agent Runtime
- MCP
- Control Plane
- SSO
- SCIM
- Developer Tools
token_urls: []
---
