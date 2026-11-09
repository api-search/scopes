---
api_specs:
- filename: api-market-api-market-api-api-openapi.yml
  format: yaml
  label: API.market API.market API
  slug: api-market-api-market-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-api-market-api-api-openapi.yml
- filename: api-market-bridgeml-api-openapi.yml
  format: yaml
  label: API.market Bridgeml API
  slug: api-market-bridgeml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-bridgeml-api-openapi.yml
- filename: api-market-images-api-openapi.yml
  format: yaml
  label: API.market Images API
  slug: api-market-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-images-api-openapi.yml
- filename: api-market-magicapi-api-openapi.yml
  format: yaml
  label: API.market Magicapi API
  slug: api-market-magicapi-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-magicapi-api-openapi.yml
- filename: api-market-mcp-api-openapi.yml
  format: yaml
  label: API.market MCP API
  slug: api-market-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-mcp-api-openapi.yml
- filename: api-market-models-api-openapi.yml
  format: yaml
  label: API.market Models API
  slug: api-market-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-models-api-openapi.yml
- filename: api-market-pipfeed-api-openapi.yml
  format: yaml
  label: API.market Pipfeed API
  slug: api-market-pipfeed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-pipfeed-api-openapi.yml
- filename: api-market-predictions-api-openapi.yml
  format: yaml
  label: API.market Predictions API
  slug: api-market-predictions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-predictions-api-openapi.yml
- filename: api-market-status-api-openapi.yml
  format: yaml
  label: API.market Status API
  slug: api-market-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-status-api-openapi.yml
- filename: api-market-subscription-api-openapi.yml
  format: yaml
  label: API.market Subscription API
  slug: api-market-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-subscription-api-openapi.yml
- filename: api-market-toonme-api-api-openapi.yml
  format: yaml
  label: API.market Toonme API
  slug: api-market-toonme-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-toonme-api-api-openapi.yml
- filename: api-market-user-api-openapi.yml
  format: yaml
  label: API.market User API
  slug: api-market-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/api-market/openapi/api-market-user-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Api Market Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'API.market publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the API.market API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: API.market
provider_slug: api-market
schemes: []
scope_count: 2
scope_names:
- mcp:use
- offline_access
scopes:
- description: Use the API.market MCP gateway (the only scope the protected-resource document for https://api.market/api/mcp/gateway lists).
  flows: []
  scope: mcp:use
- description: Issue a refresh token (grant_types_supported includes refresh_token).
  flows: []
  scope: offline_access
slug: api-market-scopes
source_filename: api-market-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: https://api.market/.well-known/oauth-authorization-server\nscopes:\n- name: mcp:use\n  description: Use the API.market MCP gateway (the only scope the protected-resource document for https://api.market/api/mcp/gateway\n    lists).\n- name: offline_access\n  description: Issue a refresh token (grant_types_supported includes refresh_token).\n"
source_yaml_url: https://artifacts.apis.io/api-market/scopes/api-market-scopes.yml
summary_line: 2 scopes
tags:
- API Marketplace
- MCP
- AI Agents
- API Monetization
- Subscription
- Usage Metering
- OAuth
- Authentication
token_bound: false
token_urls: []
---
