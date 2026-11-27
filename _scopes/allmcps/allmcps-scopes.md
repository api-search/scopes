---
api_specs:
- filename: allmcps-a2a-api-openapi.yml
  format: yaml
  label: AllMCPs A2a API
  slug: allmcps-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-a2a-api-openapi.yml
- filename: allmcps-acp-api-openapi.yml
  format: yaml
  label: AllMCPs Acp API
  slug: allmcps-acp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-acp-api-openapi.yml
- filename: allmcps-ads-api-openapi.yml
  format: yaml
  label: AllMCPs Ads API
  slug: allmcps-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-ads-api-openapi.yml
- filename: allmcps-agent-api-openapi.yml
  format: yaml
  label: AllMCPs Agent API
  slug: allmcps-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-agent-api-openapi.yml
- filename: allmcps-badge-api-openapi.yml
  format: yaml
  label: AllMCPs Badge API
  slug: allmcps-badge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-badge-api-openapi.yml
- filename: allmcps-boost-api-openapi.yml
  format: yaml
  label: AllMCPs Boost API
  slug: allmcps-boost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-boost-api-openapi.yml
- filename: allmcps-categories-api-openapi.yml
  format: yaml
  label: AllMCPs Categories API
  slug: allmcps-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-categories-api-openapi.yml
- filename: allmcps-health-api-openapi.yml
  format: yaml
  label: AllMCPs Health API
  slug: allmcps-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-health-api-openapi.yml
- filename: allmcps-mcp-api-openapi.yml
  format: yaml
  label: AllMCPs MCP API
  slug: allmcps-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-mcp-api-openapi.yml
- filename: allmcps-search-api-openapi.yml
  format: yaml
  label: AllMCPs Search API
  slug: allmcps-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-search-api-openapi.yml
- filename: allmcps-servers-api-openapi.yml
  format: yaml
  label: AllMCPs Servers API
  slug: allmcps-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-servers-api-openapi.yml
- filename: allmcps-submit-api-openapi.yml
  format: yaml
  label: AllMCPs Submit API
  slug: allmcps-submit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/allmcps/openapi/allmcps-submit-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: AllMCPs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AllMCPs publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AllMCPs API on a user''s behalf.


  Tokens are issued from https://allmcps.com/api/v1/agent/register/confirm.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AllMCPs
provider_slug: allmcps
schemes:
- description: 'Bearer token minted via POST /api/v1/agent/register + /api/v1/agent/register/confirm (email-verified, no OAuth redirect flow). Send as `Authorization: Bearer amcp_...`. Also documented at /.well-known/oauth-protected-resource and /auth.md.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://allmcps.com/api/v1/agent/register/confirm
  name: agentBearerAuth
  source: openapi/allmcps-openapi.json
scope_count: 2
scope_names:
- checkout:write
- listings:claim
scopes:
- description: 'Create, update, complete and cancel Agentic Commerce Protocol checkout sessions to buy listing boosts. Payment still needs a Stripe shared payment token the buyer granted; this scope alone cannot spend money. Required by: ACP: /api/acp/checkout_sessions (all endpoints).'
  flows:
  - clientCredentials
  scope: checkout:write
- description: 'Claim ownership of an existing MCP server listing via DNS TXT record, site verification badge, or GitHub README badge proof. Grants no other write access. Required by: POST /api/v1/agent/claim, MCP tool: verify_mcp_claim (with an agentToken).'
  flows:
  - clientCredentials
  scope: listings:claim
slug: allmcps-scopes
source_filename: allmcps-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/allmcps-openapi.json\nschemes:\n- name: agentBearerAuth\n  source: openapi/allmcps-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://allmcps.com/api/v1/agent/register/confirm\n  description: 'Bearer token minted via POST /api/v1/agent/register + /api/v1/agent/register/confirm\n    (email-verified, no OAuth redirect flow). Send as `Authorization: Bearer amcp_...`. Also\n    documented at /.well-known/oauth-protected-resource and /auth.md.'\nscopes:\n- scope: checkout:write\n  description: 'Create, update, complete and cancel Agentic Commerce Protocol checkout sessions\n    to buy listing boosts. Payment still needs a Stripe shared payment token the buyer granted;\n    this scope alone cannot spend money. Required by: ACP: /api/acp/checkout_sessions (all endpoints).'\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allmcps-openapi.json\n- scope: listings:claim\n  description: 'Claim ownership\
  \ of an existing MCP server listing via DNS TXT record, site verification\n    badge, or GitHub README badge proof. Grants no other write access. Required by: POST /api/v1/agent/claim,\n    MCP tool: verify_mcp_claim (with an agentToken).'\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/allmcps-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/allmcps/scopes/allmcps-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Directory
- MCP
- AI Agents
- Developer Tools
- Search & Data Extraction
- Finance & Fintech
- Communications
- Knowledge & Memory
token_bound: false
token_urls:
- https://allmcps.com/api/v1/agent/register/confirm
---
