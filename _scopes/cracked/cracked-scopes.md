---
api_specs:
- filename: cracked-apps-api-openapi.yml
  format: yaml
  label: Cracked API Apps API
  slug: cracked-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-apps-api-openapi.yml
- filename: cracked-auth-api-openapi.yml
  format: yaml
  label: Cracked API Auth API
  slug: cracked-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-auth-api-openapi.yml
- filename: cracked-batches-api-openapi.yml
  format: yaml
  label: Cracked API Batches API
  slug: cracked-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-batches-api-openapi.yml
- filename: cracked-datasets-api-openapi.yml
  format: yaml
  label: Cracked API Datasets API
  slug: cracked-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-datasets-api-openapi.yml
- filename: cracked-discover-api-openapi.yml
  format: yaml
  label: Cracked API Discover API
  slug: cracked-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-discover-api-openapi.yml
- filename: cracked-inspect-api-openapi.yml
  format: yaml
  label: Cracked API Inspect API
  slug: cracked-inspect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-inspect-api-openapi.yml
- filename: cracked-providers-api-openapi.yml
  format: yaml
  label: Cracked API Providers API
  slug: cracked-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-providers-api-openapi.yml
- filename: cracked-referrals-api-openapi.yml
  format: yaml
  label: Cracked API Referrals API
  slug: cracked-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-referrals-api-openapi.yml
- filename: cracked-refunds-api-openapi.yml
  format: yaml
  label: Cracked API Refunds API
  slug: cracked-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-refunds-api-openapi.yml
- filename: cracked-relay-api-openapi.yml
  format: yaml
  label: Cracked API Relay API
  slug: cracked-relay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-relay-api-openapi.yml
- filename: cracked-run-api-openapi.yml
  format: yaml
  label: Cracked API Run API
  slug: cracked-run-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-run-api-openapi.yml
- filename: cracked-runs-api-openapi.yml
  format: yaml
  label: Cracked API Runs API
  slug: cracked-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-runs-api-openapi.yml
- filename: cracked-schedules-api-openapi.yml
  format: yaml
  label: Cracked API Schedules API
  slug: cracked-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-schedules-api-openapi.yml
- filename: cracked-secrets-api-openapi.yml
  format: yaml
  label: Cracked API Secrets API
  slug: cracked-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-secrets-api-openapi.yml
- filename: cracked-wallet-api-openapi.yml
  format: yaml
  label: Cracked API Wallet API
  slug: cracked-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-wallet-api-openapi.yml
- filename: cracked-x402-api-openapi.yml
  format: yaml
  label: Cracked API X402 API
  slug: cracked-x402-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/openapi/cracked-x402-api-openapi.yml
authorization_urls:
- https://cracked.ai/oauth/authorize
description: ''
docs: https://cracked.ai/docs/mcp
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Cracked Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Cracked API publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Cracked API API on a user''s behalf.


  Tokens are issued from https://cracked.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Cracked API
provider_slug: cracked
schemes:
- flows:
  - authorizationUrl: https://cracked.ai/oauth/authorize
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://cracked.ai/oauth/register
    revocationUrl: https://cracked.ai/oauth/revoke
    tokenUrl: https://cracked.ai/oauth/token
  name: OAuth 2.1 with PKCE (MCP)
  source: well-known/cracked-oauth-authorization-server.json
scope_count: 4
scope_names:
- tools:discover
- tools:run
- wallet:read
- offline_access
scopes:
- description: Discover and inspect tools in the catalog
  flows:
  - authorizationCode
  scope: tools:discover
- description: Execute tool runs (billed per call)
  flows:
  - authorizationCode
  scope: tools:run
- description: Read wallet balance and activity
  flows:
  - authorizationCode
  scope: wallet:read
- description: Refresh-token access for long-lived MCP sessions
  flows:
  - authorizationCode
  scope: offline_access
slug: cracked-scopes
source_filename: cracked-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://cracked.ai/.well-known/oauth-authorization-server\ndocs: https://cracked.ai/docs/mcp\nschemes:\n  - name: OAuth 2.1 with PKCE (MCP)\n    source: well-known/cracked-oauth-authorization-server.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://cracked.ai/oauth/authorize\n        tokenUrl: https://cracked.ai/oauth/token\n        registrationUrl: https://cracked.ai/oauth/register\n        revocationUrl: https://cracked.ai/oauth/revoke\n        pkce: S256\nscopes:\n  - scope: tools:discover\n    description: Discover and inspect tools in the catalog\n    flows: [authorizationCode]\n    sources: [well-known/cracked-oauth-authorization-server.json, well-known/cracked-oauth-protected-resource.json]\n  - scope: tools:run\n    description: Execute tool runs (billed per call)\n    flows: [authorizationCode]\n    sources: [well-known/cracked-oauth-authorization-server.json, well-known/cracked-oauth-protected-resource.json]\n\
  \  - scope: wallet:read\n    description: Read wallet balance and activity\n    flows: [authorizationCode]\n    sources: [well-known/cracked-oauth-authorization-server.json, well-known/cracked-oauth-protected-resource.json]\n  - scope: offline_access\n    description: Refresh-token access for long-lived MCP sessions\n    flows: [authorizationCode]\n    sources: [well-known/cracked-oauth-authorization-server.json]\nnotes: >-\n  The OpenAPI declares only a bearer http scheme (ck_live_ API keys), so nothing was derivable from\n  the spec; these scopes come from the provider's live RFC 8414 authorization-server metadata and\n  RFC 9728 protected-resource metadata, both fetched 2026-09-03. OAuth is used by MCP clients;\n  plain /v1 calls use the bearer key. Scope descriptions are ours, inferred from the scope names\n  and the MCP docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cracked/refs/heads/main/scopes/cracked-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- AI Agents
- Agent Tools
- MCP
- Tool Router
- API Aggregator
- Web Search
- Web Scraping
- Data Enrichment
- llms-txt
- Agent Skills
- pay-per-call
- Aggregator
- Lead Generation
- AI Models
- Developer Tools
- lead gen
- SEO
- social-media-data
- E-Commerce
- Finance
- Weather
- A2A
token_urls:
- https://cracked.ai/oauth/token
---
