---
api_specs:
- filename: a-upgradenet-com.json
  format: json
  label: a-un API
  slug: a-un-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com.json
- filename: a-upgradenet-com-agent-account-api-openapi.yml
  format: yaml
  label: Agent Upgrade Network Agent account API
  slug: a-upgradenet-com-agent-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com-agent-account-api-openapi.yml
- filename: a-upgradenet-com-agent-identity-api-openapi.yml
  format: yaml
  label: Agent Upgrade Network Agent identity API
  slug: a-upgradenet-com-agent-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com-agent-identity-api-openapi.yml
- filename: a-upgradenet-com-authenticated-products-api-openapi.yml
  format: yaml
  label: Agent Upgrade Network Authenticated products API
  slug: a-upgradenet-com-authenticated-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com-authenticated-products-api-openapi.yml
- filename: a-upgradenet-com-discovery-api-openapi.yml
  format: yaml
  label: Agent Upgrade Network Discovery API
  slug: a-upgradenet-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com-discovery-api-openapi.yml
- filename: a-upgradenet-com-evolution-api-openapi.yml
  format: yaml
  label: Agent Upgrade Network Evolution API
  slug: a-upgradenet-com-evolution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com-evolution-api-openapi.yml
- filename: a-upgradenet-com-marketplace-api-openapi.yml
  format: yaml
  label: Agent Upgrade Network Marketplace API
  slug: a-upgradenet-com-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com-marketplace-api-openapi.yml
- filename: a-upgradenet-com-mcp-api-openapi.yml
  format: yaml
  label: Agent Upgrade Network MCP API
  slug: a-upgradenet-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com-mcp-api-openapi.yml
- filename: a-upgradenet-com-pay-per-call-api-openapi.yml
  format: yaml
  label: Agent Upgrade Network Pay per call API
  slug: a-upgradenet-com-pay-per-call-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com-pay-per-call-api-openapi.yml
- filename: a-upgradenet-com-upgrades-api-openapi.yml
  format: yaml
  label: Agent Upgrade Network Upgrades API
  slug: a-upgradenet-com-upgrades-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/a-upgradenet-com/openapi/a-upgradenet-com-upgrades-api-openapi.yml
authorization_urls:
- https://2pr.io/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: A Upgradenet Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Agent Upgrade Network publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agent Upgrade Network API on a user''s behalf.


  Tokens are issued from https://2pr.io/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agent Upgrade Network
provider_slug: a-upgradenet-com
schemes:
- description: '"Sign in with 2pr". Authorization code with PKCE S256; register a client first.'
  flows:
  - authorizationUrl: https://2pr.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://2pr.io/api/oauth/token
  name: oauth2
  source: openapi/a-upgradenet-com-openapi.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Call the 2pr.io MCP tools on behalf of the signed-in user.
  flows:
  - authorizationCode
  scope: mcp
slug: a-upgradenet-com-scopes
source_filename: a-upgradenet-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/a-upgradenet-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/a-upgradenet-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://2pr.io/oauth/authorize\n    tokenUrl: https://2pr.io/api/oauth/token\n  description: '\"Sign in with 2pr\". Authorization code with PKCE S256; register a client first.'\nscopes:\n- scope: mcp\n  description: Call the 2pr.io MCP tools on behalf of the signed-in user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/a-upgradenet-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/a-upgradenet-com/scopes/a-upgradenet-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- AI Agent Upgrades
- USDC Payments
token_bound: false
token_urls:
- https://2pr.io/api/oauth/token
---
