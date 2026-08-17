---
api_specs:
- filename: gojiberry-ai-appexternal-api-openapi.yml
  format: yaml
  label: Gojiberry AI AppExternal API
  slug: gojiberry-ai-appexternal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-appexternal-api-openapi.yml
- filename: gojiberry-ai-campaigns-api-openapi.yml
  format: yaml
  label: Gojiberry AI Campaigns API
  slug: gojiberry-ai-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-campaigns-api-openapi.yml
- filename: gojiberry-ai-contacts-api-openapi.yml
  format: yaml
  label: Gojiberry AI Contacts API
  slug: gojiberry-ai-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-contacts-api-openapi.yml
- filename: gojiberry-ai-lead-source-agents-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lead source agents API
  slug: gojiberry-ai-lead-source-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lead-source-agents-api-openapi.yml
- filename: gojiberry-ai-lists-api-openapi.yml
  format: yaml
  label: Gojiberry AI Lists API
  slug: gojiberry-ai-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-lists-api-openapi.yml
- filename: gojiberry-ai-organization-api-openapi.yml
  format: yaml
  label: Gojiberry AI Organization API
  slug: gojiberry-ai-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-organization-api-openapi.yml
- filename: gojiberry-ai-unibox-api-openapi.yml
  format: yaml
  label: Gojiberry AI Unibox API
  slug: gojiberry-ai-unibox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-unibox-api-openapi.yml
- filename: gojiberry-ai-user-api-openapi.yml
  format: yaml
  label: Gojiberry AI User API
  slug: gojiberry-ai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/openapi/gojiberry-ai-user-api-openapi.yml
authorization_urls:
- https://mcp.gojiberry.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Gojiberry Ai Scopes
name_suffix: OAuth Scopes
note: The External REST API at ext.gojiberry.ai has NO OAuth surface — it is a bearer API key (JWT) only, so derive-oauth-scopes.py finds zero oauth2 securitySchemes in the OpenAPI. The OAuth scopes recorded here belong to the hosted MCP server at mcp.gojiberry.ai, which publishes RFC 8414 authorization server metadata and RFC 9728 protected resource metadata anonymously. Gojiberry publishes no human-readable scope reference page; these values are read verbatim from the machine-readable metadata.
overview: 'Gojiberry AI publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gojiberry AI API on a user''s behalf.


  Tokens are issued from https://mcp.gojiberry.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gojiberry AI
provider_slug: gojiberry-ai
schemes:
- dynamic_client_registration: https://mcp.gojiberry.ai/register
  flows:
  - authorizationUrl: https://mcp.gojiberry.ai/authorize
    flow: authorizationCode
    grant_types:
    - authorization_code
    - refresh_token
    pkce:
    - S256
    - plain
    tokenUrl: https://mcp.gojiberry.ai/token
    token_endpoint_auth_methods:
    - none
    - client_secret_post
  issuer: https://mcp.gojiberry.ai
  name: MCP OAuth 2.1
  source: well-known/gojiberry-ai-oauth-authorization-server.json
  surface: mcp
scope_count: 2
scope_names:
- mcp:tools
- claudeai
scopes:
- description: Advertised scope granting an MCP client access to the Gojiberry tool surface. No published description; name read from scopes_supported.
  flows:
  - authorizationCode
  scope: mcp:tools
- description: Advertised scope used by the Claude MCP connector flow documented at https://gojiberry.ai/how-to-do-outreach-claude-linkedin-mcp. No published description; name read from scopes_supported.
  flows:
  - authorizationCode
  scope: claudeai
slug: gojiberry-ai-scopes
source_filename: gojiberry-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.gojiberry.ai/.well-known/oauth-authorization-server\nnote: >-\n  The External REST API at ext.gojiberry.ai has NO OAuth surface — it is a\n  bearer API key (JWT) only, so derive-oauth-scopes.py finds zero oauth2\n  securitySchemes in the OpenAPI. The OAuth scopes recorded here belong to the\n  hosted MCP server at mcp.gojiberry.ai, which publishes RFC 8414 authorization\n  server metadata and RFC 9728 protected resource metadata anonymously. Gojiberry\n  publishes no human-readable scope reference page; these values are read\n  verbatim from the machine-readable metadata.\nschemes:\n- name: MCP OAuth 2.1\n  surface: mcp\n  source: well-known/gojiberry-ai-oauth-authorization-server.json\n  issuer: https://mcp.gojiberry.ai\n  dynamic_client_registration: https://mcp.gojiberry.ai/register  # RFC 7591\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.gojiberry.ai/authorize\n    tokenUrl: https://mcp.gojiberry.ai/token\n\
  \    pkce: [S256, plain]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none, client_secret_post]\nscopes:\n- scope: mcp:tools\n  description: >-\n    Advertised scope granting an MCP client access to the Gojiberry tool\n    surface. No published description; name read from scopes_supported.\n  flows: [authorizationCode]\n  sources: [well-known/gojiberry-ai-oauth-authorization-server.json]\n- scope: claudeai\n  description: >-\n    Advertised scope used by the Claude MCP connector flow documented at\n    https://gojiberry.ai/how-to-do-outreach-claude-linkedin-mcp. No published\n    description; name read from scopes_supported.\n  flows: [authorizationCode]\n  sources: [well-known/gojiberry-ai-oauth-authorization-server.json]\ngaps:\n- No scopes/permissions reference page is published on the docs site.\n- The REST External API has no scope model; access is all-or-nothing per API key,\n  with organization-owner impersonation via x-impersonate-user-id.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gojiberry-ai/refs/heads/main/scopes/gojiberry-ai-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Company
- Sales
- Lead Generation
- Sales Intelligence
- AI Agents
- Outbound
- Go-To-Market
- Prospecting
- LinkedIn
- CRM
token_urls:
- https://mcp.gojiberry.ai/token
---
