---
api_specs:
- filename: alterestate-openapi.yml
  format: yaml
  label: AlterEstate API
  slug: alterestate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alterestate/refs/heads/main/openapi/alterestate-openapi.yml
authorization_urls:
- https://secure.alterestate.com/oauth/authorize/
description: ''
docs: https://secure.alterestate.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Alterestate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AlterEstate publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AlterEstate API on a user''s behalf.


  Tokens are issued from https://secure.alterestate.com/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AlterEstate
provider_slug: alterestate
schemes:
- description: OAuth 2.0 authorization used by the AlterEstate (Brik/alterai) hosted MCP server.
  flows:
  - authorizationUrl: https://secure.alterestate.com/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://secure.alterestate.com/oauth/token/
  name: oauth2
  source: openapi/alterestate-openapi.yml
scope_count: 1
scope_names:
- mcp
scopes:
- description: Access the AlterEstate hosted MCP server (secure.alterestate.com/api/v1/alterai/mcp/).
  flows:
  - authorizationCode
  scope: mcp
slug: alterestate-scopes
source_filename: alterestate-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/alterestate-openapi.yml\ndocs: https://secure.alterestate.com/.well-known/oauth-authorization-server\nschemes:\n- name: oauth2\n  source: openapi/alterestate-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.alterestate.com/oauth/authorize/\n    tokenUrl: https://secure.alterestate.com/oauth/token/\n  description: OAuth 2.0 authorization used by the AlterEstate (Brik/alterai) hosted MCP server.\nscopes:\n- scope: mcp\n  description: Access the AlterEstate hosted MCP server (secure.alterestate.com/api/v1/alterai/mcp/).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/alterestate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alterestate/refs/heads/main/scopes/alterestate-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Real Estate
- CRM
- Property Management
- Lead Management
- Latin America
- SaaS
- Artificial Intelligence
- MCP
token_urls:
- https://secure.alterestate.com/oauth/token/
---
