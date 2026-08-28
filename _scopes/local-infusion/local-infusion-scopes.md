---
api_specs:
- filename: local-infusion-wp-v2-api-openapi.yml
  format: yaml
  label: Local Infusion WordPress Content API
  slug: local-infusion-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-wp-v2-api-openapi.yml
- filename: local-infusion-mcp-api-openapi.yml
  format: yaml
  label: Local Infusion MCP API
  slug: local-infusion-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-mcp-api-openapi.yml
- filename: local-infusion-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: Local Infusion WordPress Abilities API
  slug: local-infusion-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-wp-abilities-v1-api-openapi.yml
- filename: local-infusion-root-api-openapi.yml
  format: yaml
  label: Local Infusion WordPress Root API
  slug: local-infusion-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-root-api-openapi.yml
- filename: local-infusion-oembed-1-0-api-openapi.yml
  format: yaml
  label: Local Infusion oEmbed API
  slug: local-infusion-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/openapi/local-infusion-oembed-1-0-api-openapi.yml
authorization_urls:
- https://mylocalinfusion.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Local Infusion Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Local Infusion publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Local Infusion API on a user''s behalf.


  Tokens are issued from https://mylocalinfusion.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Local Infusion
provider_slug: local-infusion
schemes:
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched 2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://mylocalinfusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mylocalinfusion.com/oauth/token
  name: mcpOAuth2
  source: openapi/local-infusion-mcp-api-openapi.yml
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched 2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://mylocalinfusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mylocalinfusion.com/oauth/token
  name: mcpOAuth2
  source: openapi/local-infusion-oembed-1-0-api-openapi.yml
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched 2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://mylocalinfusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mylocalinfusion.com/oauth/token
  name: mcpOAuth2
  source: openapi/local-infusion-root-api-openapi.yml
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched 2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://mylocalinfusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mylocalinfusion.com/oauth/token
  name: mcpOAuth2
  source: openapi/local-infusion-wp-abilities-v1-api-openapi.yml
- description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC 8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched 2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.
  flows:
  - authorizationUrl: https://mylocalinfusion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://mylocalinfusion.com/oauth/token
  name: mcpOAuth2
  source: openapi/local-infusion-wp-v2-api-openapi.yml
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the site's Model Context Protocol server.
  flows:
  - authorizationCode
  scope: mcp
slug: local-infusion-scopes
source_filename: local-infusion-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: derived\nsource: openapi/local-infusion-mcp-api-openapi.yml, openapi/local-infusion-oembed-1-0-api-openapi.yml,\n  openapi/local-infusion-root-api-openapi.yml, openapi/local-infusion-wp-abilities-v1-api-openapi.yml,\n  openapi/local-infusion-wp-v2-api-openapi.yml\nschemes:\n- name: mcpOAuth2\n  source: openapi/local-infusion-mcp-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mylocalinfusion.com/oauth/authorize\n    tokenUrl: https://mylocalinfusion.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched\n    2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata\n    names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.\n- name: mcpOAuth2\n  source: openapi/local-infusion-oembed-1-0-api-openapi.yml\n  flows:\n\
  \  - flow: authorizationCode\n    authorizationUrl: https://mylocalinfusion.com/oauth/authorize\n    tokenUrl: https://mylocalinfusion.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched\n    2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata\n    names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.\n- name: mcpOAuth2\n  source: openapi/local-infusion-root-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mylocalinfusion.com/oauth/authorize\n    tokenUrl: https://mylocalinfusion.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched\n    2026-08-25, HTTP 200). Guards the `mcp` namespace; the\
  \ RFC 9728 protected-resource metadata\n    names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.\n- name: mcpOAuth2\n  source: openapi/local-infusion-wp-abilities-v1-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mylocalinfusion.com/oauth/authorize\n    tokenUrl: https://mylocalinfusion.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE (S256), as advertised by the provider's RFC\n    8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched\n    2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata\n    names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.\n- name: mcpOAuth2\n  source: openapi/local-infusion-wp-v2-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mylocalinfusion.com/oauth/authorize\n    tokenUrl: https://mylocalinfusion.com/oauth/token\n  description: OAuth 2.1 authorization-code + PKCE\
  \ (S256), as advertised by the provider's RFC\n    8414 metadata at https://mylocalinfusion.com/.well-known/oauth-authorization-server (fetched\n    2026-08-25, HTTP 200). Guards the `mcp` namespace; the RFC 9728 protected-resource metadata\n    names https://mylocalinfusion.com/wp-json/mcp/mcp-oauth-server.\nscopes:\n- scope: mcp\n  description: Access the site's Model Context Protocol server.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/local-infusion-mcp-api-openapi.yml\n  - openapi/local-infusion-oembed-1-0-api-openapi.yml\n  - openapi/local-infusion-root-api-openapi.yml\n  - openapi/local-infusion-wp-abilities-v1-api-openapi.yml\n  - openapi/local-infusion-wp-v2-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/local-infusion/refs/heads/main/scopes/local-infusion-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Healthcare
- Health Services
- Infusion Therapy
- Specialty Pharmacy
- Ambulatory Care
- Patient Services
- Autoimmune
- Chronic Care
- MCP
- WordPress
token_urls:
- https://mylocalinfusion.com/oauth/token
---
