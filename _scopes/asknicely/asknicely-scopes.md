---
api_specs:
- filename: asknicely-contacts-api-openapi.yml
  format: yaml
  label: AskNicely Contacts API
  slug: asknicely-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-contacts-api-openapi.yml
- filename: asknicely-in-app-surveys-api-openapi.yml
  format: yaml
  label: AskNicely In-App Surveys API
  slug: asknicely-in-app-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-in-app-surveys-api-openapi.yml
- filename: asknicely-responses-api-openapi.yml
  format: yaml
  label: AskNicely Responses API
  slug: asknicely-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-responses-api-openapi.yml
- filename: asknicely-statistics-api-openapi.yml
  format: yaml
  label: AskNicely Statistics API
  slug: asknicely-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-statistics-api-openapi.yml
- filename: asknicely-surveys-api-openapi.yml
  format: yaml
  label: AskNicely Surveys API
  slug: asknicely-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/openapi/asknicely-surveys-api-openapi.yml
authorization_urls:
- https://mcp.asknice.ly/authorize
description: AskNicely's REST API is API-key authenticated and has no OAuth surface. The only OAuth surface AskNicely operates is the authorization server fronting its remote MCP server (Ask NiceAI), which advertises a single coarse scope. There is no published scopes/permissions reference page — the scope set below is read verbatim from the RFC 8414 authorization-server metadata document.
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Asknicely Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AskNicely publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AskNicely API on a user''s behalf.


  Tokens are issued from https://mcp.asknice.ly/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AskNicely
provider_slug: asknicely
schemes:
- dynamic_client_registration: https://mcp.asknice.ly/register
  flows:
  - authorizationUrl: https://mcp.asknice.ly/authorize
    flow: authorizationCode
    pkce:
    - S256
    refresh: true
    tokenUrl: https://mcp.asknice.ly/token
  issuer: https://mcp.asknice.ly
  name: MCP OAuth 2.1
  revocation: https://mcp.asknice.ly/revoke
  source: https://mcp.asknice.ly/.well-known/oauth-authorization-server
scope_count: 1
scope_names:
- tools
scopes:
- description: Access the Ask NiceAI MCP tool surface. AskNicely advertises exactly one scope; there is no read/write or per-resource scope decomposition, so consent is all-or-nothing over the tool set.
  flows:
  - authorizationCode
  scope: tools
slug: asknicely-scopes
source_filename: asknicely-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://mcp.asknice.ly/.well-known/oauth-authorization-server\ndescription: >-\n  AskNicely's REST API is API-key authenticated and has no OAuth surface. The only OAuth surface AskNicely\n  operates is the authorization server fronting its remote MCP server (Ask NiceAI), which advertises a\n  single coarse scope. There is no published scopes/permissions reference page — the scope set below is\n  read verbatim from the RFC 8414 authorization-server metadata document.\napplies_to: AskNicely MCP Server (Ask NiceAI)\nschemes:\n- name: MCP OAuth 2.1\n  source: https://mcp.asknice.ly/.well-known/oauth-authorization-server\n  issuer: https://mcp.asknice.ly\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.asknice.ly/authorize\n    tokenUrl: https://mcp.asknice.ly/token\n    pkce: [S256]\n    refresh: true\n  dynamic_client_registration: https://mcp.asknice.ly/register\n  revocation: https://mcp.asknice.ly/revoke\n\
  scopes:\n- scope: tools\n  description: >-\n    Access the Ask NiceAI MCP tool surface. AskNicely advertises exactly one scope; there is no\n    read/write or per-resource scope decomposition, so consent is all-or-nothing over the tool set.\n  flows: [authorizationCode]\n  sources: ['https://mcp.asknice.ly/.well-known/oauth-authorization-server']\nprotected_resources:\n- resource: https://nicely.asknice.ly/mcp\n  authorization_servers: [https://mcp.asknice.ly]\n  scopes_supported: [tools]\n  bearer_methods_supported: [header]\n  source: https://mcp.asknice.ly/.well-known/oauth-protected-resource\ngaps:\n- No scopes or permissions reference page in AskNicely's documentation.\n- A single `tools` scope means no least-privilege decomposition for agent consent.\n- The REST API has no OAuth option at all; it is a single account-wide API key with no scoping.\nx-evidence:\n- {url: 'https://mcp.asknice.ly/.well-known/oauth-authorization-server', http_status: 200, fetched: '2026-08-06'}\n- {url:\
  \ 'https://mcp.asknice.ly/.well-known/oauth-protected-resource', http_status: 200, fetched: '2026-08-06'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asknicely/refs/heads/main/scopes/asknicely-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Customer Experience
- NPS
- Surveys
- Feedback
- Reputation Management
- Software-as-a-Service
- Customer Success
- Reviews
- SMS
token_urls:
- https://mcp.asknice.ly/token
---
