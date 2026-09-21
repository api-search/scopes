---
api_specs:
- filename: phoslabs-io-openapi.yml
  format: yaml
  label: Behavioral Science API
  slug: behavioral-science-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/openapi/phoslabs-io-openapi.yml
authorization_urls:
- https://mcp.phoslabs.io/authorize
description: ''
docs: https://mcp.phoslabs.io/.well-known/oauth-protected-resource/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Phoslabs Io Scopes
name_suffix: OAuth Scopes
note: The OpenAPI declares no oauth2 scheme (derive-oauth-scopes.py found nothing), but the MCP server documents OAuth 2.1 through its RFC 8414 / RFC 9728 discovery documents, which are the provider's only published scope reference. One scope is declared and no human description of it is published anywhere; the name suggests it exists to satisfy the Claude connector flow. No scopes reference page exists (/docs is 403).
overview: 'Phos Labs publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Phos Labs API on a user''s behalf.


  Tokens are issued from https://mcp.phoslabs.io/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Phos Labs
provider_slug: phoslabs-io
schemes:
- bearer_methods:
  - header
  flows:
  - authorizationUrl: https://mcp.phoslabs.io/authorize
    flow: authorizationCode
    pkce:
    - S256
    refreshUrl: https://mcp.phoslabs.io/token
    tokenUrl: https://mcp.phoslabs.io/token
  issuer: https://mcp.phoslabs.io/
  name: mcp-oauth
  registration_endpoint: https://mcp.phoslabs.io/register
  resource: https://mcp.phoslabs.io/mcp
  revocation_endpoint: https://mcp.phoslabs.io/revoke
  source: well-known/phoslabs-io-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - none
  type: oauth2
scope_count: 1
scope_names:
- claudeai
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: claudeai
slug: phoslabs-io-scopes
source_filename: phoslabs-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: https://mcp.phoslabs.io/.well-known/oauth-authorization-server\ndocs: https://mcp.phoslabs.io/.well-known/oauth-protected-resource/mcp\nnote: >-\n  The OpenAPI declares no oauth2 scheme (derive-oauth-scopes.py found nothing), but the MCP server documents\n  OAuth 2.1 through its RFC 8414 / RFC 9728 discovery documents, which are the provider's only published\n  scope reference. One scope is declared and no human description of it is published anywhere; the name\n  suggests it exists to satisfy the Claude connector flow. No scopes reference page exists (/docs is 403).\nschemes:\n- name: mcp-oauth\n  type: oauth2\n  source: well-known/phoslabs-io-oauth-authorization-server.json\n  issuer: https://mcp.phoslabs.io/\n  resource: https://mcp.phoslabs.io/mcp\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.phoslabs.io/authorize\n    tokenUrl: https://mcp.phoslabs.io/token\n    refreshUrl: https://mcp.phoslabs.io/token\n\
  \    pkce: [S256]\n  registration_endpoint: https://mcp.phoslabs.io/register\n  revocation_endpoint: https://mcp.phoslabs.io/revoke\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic, none]\n  bearer_methods: [header]\nscopes:\n- scope: claudeai\n  description: null\n  flows: [authorizationCode]\n  sources: [well-known/phoslabs-io-oauth-authorization-server.json, well-known/phoslabs-io-oauth-protected-resource.json]\n  note: Declared in scopes_supported of both discovery documents; no published description.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phoslabs-io/refs/heads/main/scopes/phoslabs-io-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Behavioral Science
- Conversion Optimization
- E-Commerce
- Pricing
- Copywriting
- AI Agents
- MCP
- A2A
- Decision Intelligence
- Agentic Commerce
token_urls:
- https://mcp.phoslabs.io/token
---
