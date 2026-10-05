---
api_specs:
- filename: gameball-batches-api-openapi.yml
  format: yaml
  label: Gameball Batches API
  slug: gameball-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/openapi/gameball-batches-api-openapi.yml
- filename: gameball-customers-api-openapi.yml
  format: yaml
  label: Gameball Customers API
  slug: gameball-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/openapi/gameball-customers-api-openapi.yml
- filename: gameball-events-api-openapi.yml
  format: yaml
  label: Gameball Events API
  slug: gameball-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/openapi/gameball-events-api-openapi.yml
- filename: gameball-gameball-api-api-openapi.yml
  format: yaml
  label: Gameball API
  slug: gameball-gameball-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/openapi/gameball-gameball-api-api-openapi.yml
- filename: gameball-integrations-api-openapi.yml
  format: yaml
  label: Gameball Integrations API
  slug: gameball-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/openapi/gameball-integrations-api-openapi.yml
- filename: gameball-orders-api-openapi.yml
  format: yaml
  label: Gameball Orders API
  slug: gameball-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/openapi/gameball-orders-api-openapi.yml
- filename: gameball-payments-api-openapi.yml
  format: yaml
  label: Gameball Payments API
  slug: gameball-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/openapi/gameball-payments-api-openapi.yml
- filename: gameball-plants-api-openapi.yml
  format: yaml
  label: Gameball Plants API
  slug: gameball-plants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/openapi/gameball-plants-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Gameball Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gameball publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gameball API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gameball
provider_slug: gameball
schemes: []
scope_count: 1
scope_names:
- mcp
scopes:
- description: The single scope advertised in scopes_supported by both the RFC 8414 authorization-server metadata and the RFC 9728 protected-resource metadata. Gameball publishes no finer-grained scope model — one scope grants access to the whole 54-tool MCP surface, which includes destructive operations (delete_reward_campaign, delete_redemption_option, delete_custom_earning_rule, deduct_customer_points).
  flows: []
  scope: mcp
slug: gameball-scopes
source_filename: gameball-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://mcp.gameball.co/.well-known/oauth-authorization-server\nchecked: '2026-08-13'\napplies_to: Gameball MCP Server (https://mcp.gameball.co/mcp)\nnot_applicable_to: >-\n  The Gameball REST API v4.0 does NOT use OAuth. It authenticates with the\n  APIKey / SecretKey headers and declares no oauth2 securityScheme in\n  openapi/gameball-openapi.json, so it has no scope model at all. See\n  authentication/gameball-authentication.yml.\nauthorization_server:\n  issuer: https://mcp.gameball.co/\n  authorization_endpoint: https://mcp.gameball.co/authorize\n  token_endpoint: https://mcp.gameball.co/token\n  registration_endpoint: https://mcp.gameball.co/register\n  revocation_endpoint: https://mcp.gameball.co/revoke\n  grant_types_supported: [authorization_code, refresh_token]\n  response_types_supported: [code]\n  code_challenge_methods_supported: [S256]\n  token_endpoint_auth_methods_supported: [client_secret_post, none]\n  dynamic_client_registration:\
  \ true\nprotected_resource:\n  resource: https://mcp.gameball.co/\n  resource_name: Gameball MCP\n  authorization_servers: [https://mcp.gameball.co/]\nscope_count: 1\nscopes:\n  - name: mcp\n    description: >-\n      The single scope advertised in scopes_supported by both the RFC 8414\n      authorization-server metadata and the RFC 9728 protected-resource\n      metadata. Gameball publishes no finer-grained scope model — one scope\n      grants access to the whole 54-tool MCP surface, which includes destructive\n      operations (delete_reward_campaign, delete_redemption_option,\n      delete_custom_earning_rule, deduct_customer_points).\n    source: https://mcp.gameball.co/.well-known/oauth-authorization-server\nfinding: >-\n  A single coarse scope with no read/write or per-resource split. An agent\n  granted \"mcp\" can read customer data and also delete campaigns and deduct\n  customer points. There is no documented way for a client to request a\n  narrower grant.\nevidence:\n  -\
  \ url: https://mcp.gameball.co/.well-known/oauth-authorization-server\n    http_status: 200\n  - url: https://mcp.gameball.co/.well-known/oauth-protected-resource\n    http_status: 200\ndocs: null\ndocs_note: >-\n  No scopes/permissions reference page was found on docs.gameball.co; the scope\n  model is only discoverable from the two well-known metadata documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gameball/refs/heads/main/scopes/gameball-scopes.yml
summary_line: 1 scope
tags:
- Company
- Loyalty
- Rewards
- Gamification
- Customer Engagement
- Retention
- Referrals
- Marketing
- E-Commerce
- A2A
- Loyalty & Incentives
token_bound: false
token_urls: []
---
