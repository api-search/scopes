---
api_specs:
- filename: getclerion-com-deploys-api-openapi.yml
  format: yaml
  label: Clerion Deploys API
  slug: getclerion-com-deploys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclerion-com/openapi/getclerion-com-deploys-api-openapi.yml
- filename: getclerion-com-discovery-api-openapi.yml
  format: yaml
  label: Clerion Discovery API
  slug: getclerion-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclerion-com/openapi/getclerion-com-discovery-api-openapi.yml
- filename: getclerion-com-mcp-api-openapi.yml
  format: yaml
  label: Clerion MCP API
  slug: getclerion-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getclerion-com/openapi/getclerion-com-mcp-api-openapi.yml
authorization_urls:
- https://api.getclerion.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Clerion Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Clerion publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clerion API on a user''s behalf.


  Tokens are issued from https://api.getclerion.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clerion
provider_slug: getclerion-com
schemes:
- description: 'OAuth 2.1 for MCP clients: authorization code with PKCE, dynamic client registration at /oauth/register. Discover it at /.well-known/oauth-authorization-server.'
  flows:
  - authorizationUrl: https://api.getclerion.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.getclerion.com/oauth/token
  name: oauth
  source: openapi/getclerion-com-openapi.json
scope_count: 1
scope_names:
- analytics:read
scopes:
- description: Read aggregate analytics for the sites on the account. Nothing can be changed or deleted.
  flows:
  - authorizationCode
  scope: analytics:read
slug: getclerion-com-scopes
source_filename: getclerion-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: derived\nsource: openapi/getclerion-com-openapi.json\nschemes:\n- name: oauth\n  source: openapi/getclerion-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.getclerion.com/oauth/authorize\n    tokenUrl: https://api.getclerion.com/oauth/token\n  description: 'OAuth 2.1 for MCP clients: authorization code with PKCE, dynamic client registration\n    at /oauth/register. Discover it at /.well-known/oauth-authorization-server.'\nscopes:\n- scope: analytics:read\n  description: Read aggregate analytics for the sites on the account. Nothing can be changed\n    or deleted.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/getclerion-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getclerion-com/scopes/getclerion-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Artificial Intelligence
- Analytics
- Website Intelligence
- Founders
- Marketing
token_bound: false
token_urls:
- https://api.getclerion.com/oauth/token
---
