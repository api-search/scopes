---
api_specs:
- filename: brightedge-auth-api-openapi.yml
  format: yaml
  label: BrightEdge Auth API
  slug: brightedge-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-auth-api-openapi.yml
- filename: brightedge-authorize-api-openapi.yml
  format: yaml
  label: BrightEdge Authorize API
  slug: brightedge-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-authorize-api-openapi.yml
- filename: brightedge-feedback-api-openapi.yml
  format: yaml
  label: BrightEdge Feedback API
  slug: brightedge-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-feedback-api-openapi.yml
- filename: brightedge-oauth-api-openapi.yml
  format: yaml
  label: BrightEdge OAuth API
  slug: brightedge-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-oauth-api-openapi.yml
- filename: brightedge-ping-api-openapi.yml
  format: yaml
  label: BrightEdge Ping API
  slug: brightedge-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-ping-api-openapi.yml
- filename: brightedge-saml-api-openapi.yml
  format: yaml
  label: BrightEdge SAML API
  slug: brightedge-saml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-saml-api-openapi.yml
- filename: brightedge-sso-api-openapi.yml
  format: yaml
  label: BrightEdge SSO API
  slug: brightedge-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-sso-api-openapi.yml
- filename: brightedge-token-api-openapi.yml
  format: yaml
  label: BrightEdge Token API
  slug: brightedge-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-token-api-openapi.yml
- filename: brightedge-well-known-api-openapi.yml
  format: yaml
  label: BrightEdge .well Known API
  slug: brightedge-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/openapi/brightedge-well-known-api-openapi.yml
authorization_urls:
- https://mcp2.brightedge.com/authorize
- https://mcp.brightedge.com/authorize
description: ''
docs: https://www.brightedge.com/brightedge-mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Brightedge Scopes
name_suffix: OAuth Scopes
note: The REST Platform API v5.0 declares NO oauth2 securityScheme — it is key/basic/session auth only, so it has no scope surface. The OAuth surface belongs entirely to the BrightEdge MCP server, whose RFC 8414 / RFC 9728 / OIDC discovery documents were fetched anonymously (all HTTP 200) and whose setup guides publish the scope string clients must request. Scopes below are exactly what those documents and pages state; none were inferred.
overview: 'BrightEdge publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BrightEdge API on a user''s behalf.


  Tokens are issued from https://mcp2.brightedge.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BrightEdge
provider_slug: brightedge
schemes:
- flows:
  - authorizationUrl: https://mcp2.brightedge.com/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcp2.brightedge.com/token
    token_endpoint_auth_methods_supported:
    - none
  identity_provider: Auth0 (mrkt-0365.us.auth0.com)
  name: brightedge-mcp-oauth
  source: https://mcp2.brightedge.com/.well-known/oauth-authorization-server
  type: oauth2
- flows:
  - authorizationUrl: https://mcp.brightedge.com/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://mcp.brightedge.com/token
  name: brightedge-mcp-marketplace-oauth
  source: https://mcp.brightedge.com/.well-known/oauth-authorization-server
  type: oauth2
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OpenID Connect subject identity; the only scope the protected-resource metadata advertises as supported for the MCP resource.
  flows:
  - authorizationCode
  scope: openid
- description: Auth0 profile claims. Documented as part of the scope string clients send when registering the BrightEdge MCP connector (Gemini Enterprise, Microsoft Copilot Studio, Relevance AI setup guides all state "Scope openid profile email").
  flows:
  - authorizationCode
  scope: profile
- description: Auth0 email claim. Same source as profile.
  flows:
  - authorizationCode
  scope: email
slug: brightedge-scopes
source_filename: brightedge-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://www.brightedge.com/brightedge-mcp\nprobe: true\ndocs: https://www.brightedge.com/brightedge-mcp\nnote: >-\n  The REST Platform API v5.0 declares NO oauth2 securityScheme — it is key/basic/session auth only,\n  so it has no scope surface. The OAuth surface belongs entirely to the BrightEdge MCP server, whose\n  RFC 8414 / RFC 9728 / OIDC discovery documents were fetched anonymously (all HTTP 200) and whose\n  setup guides publish the scope string clients must request. Scopes below are exactly what those\n  documents and pages state; none were inferred.\nschemes:\n- name: brightedge-mcp-oauth\n  type: oauth2\n  source: https://mcp2.brightedge.com/.well-known/oauth-authorization-server\n  identity_provider: Auth0 (mrkt-0365.us.auth0.com)\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp2.brightedge.com/authorize\n    tokenUrl: https://mcp2.brightedge.com/token\n    pkce: S256\n    token_endpoint_auth_methods_supported:\
  \ [none]\n- name: brightedge-mcp-marketplace-oauth\n  type: oauth2\n  source: https://mcp.brightedge.com/.well-known/oauth-authorization-server\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.brightedge.com/authorize\n    tokenUrl: https://mcp.brightedge.com/token\n    pkce: S256\nscopes:\n- scope: openid\n  description: OpenID Connect subject identity; the only scope the protected-resource metadata\n    advertises as supported for the MCP resource.\n  flows: [authorizationCode]\n  sources:\n  - https://mcp2.brightedge.com/.well-known/oauth-protected-resource\n  - https://mcp2.brightedge.com/.well-known/oauth-authorization-server\n  - https://mcp.brightedge.com/.well-known/oauth-protected-resource\n  - https://mcp2-sse.brightedge.com/.well-known/oauth-protected-resource\n- scope: profile\n  description: Auth0 profile claims. Documented as part of the scope string clients send when\n    registering the BrightEdge MCP connector (Gemini Enterprise, Microsoft Copilot\
  \ Studio,\n    Relevance AI setup guides all state \"Scope openid profile email\").\n  flows: [authorizationCode]\n  sources:\n  - https://www.brightedge.com/brightedge-mcp\n  - https://mcp2.brightedge.com/.well-known/openid-configuration\n- scope: email\n  description: Auth0 email claim. Same source as profile.\n  flows: [authorizationCode]\n  sources:\n  - https://www.brightedge.com/brightedge-mcp\n  - https://mcp2.brightedge.com/.well-known/openid-configuration\nauthorization_server_scopes_supported:\n  note: The Auth0-backed OIDC discovery document advertises the standard Auth0 claim scope set.\n    These are identity claims, not BrightEdge data permissions — BrightEdge publishes no\n    per-tool or per-dataset scope vocabulary.\n  source: well-known/brightedge-mcp2-openid-configuration.json\n  scopes: [openid, profile, offline_access, name, given_name, family_name, nickname, email,\n    email_verified, picture, created_at, identities, phone, address]\ngaps:\n- No BrightEdge-specific\
  \ data scopes (e.g. read:keywords, read:datacube) are published; the MCP\n  server is described as read-only for the whole connected account rather than scoped per dataset.\n- Client credentials are not self-serve. The OAuth Client ID/Secret must be requested from a\n  BrightEdge Customer Success Manager or integrations@brightedge.com, and redirect URLs must be\n  allowlisted by BrightEdge before a connector will authenticate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brightedge/refs/heads/main/scopes/brightedge-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- SEO
- Search
- Content
- Marketing
- Analytics
- Keywords
- Enterprise
- AI Search
token_bound: false
token_urls:
- https://mcp2.brightedge.com/token
- https://mcp.brightedge.com/token
---
