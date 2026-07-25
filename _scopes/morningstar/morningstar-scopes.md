---
api_specs:
- filename: morningstar-oauth-api-openapi.yml
  format: yaml
  label: Morningstar Authentication API
  slug: morningstar-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-oauth-api-openapi.yml
- filename: morningstar-corporate-actions-api-openapi.yml
  format: yaml
  label: Morningstar Time Series API
  slug: morningstar-time-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-corporate-actions-api-openapi.yml
- filename: morningstar-data-points-api-openapi.yml
  format: yaml
  label: Morningstar Screener APIs
  slug: morningstar-screener-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-data-points-api-openapi.yml
- filename: morningstar-aggregates-financials-api-openapi.yml
  format: yaml
  label: Morningstar Investment Details APIs
  slug: morningstar-investment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-aggregates-financials-api-openapi.yml
- filename: morningstar-investment-list-api-openapi.yml
  format: yaml
  label: Morningstar Investment List API
  slug: morningstar-investment-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-investment-list-api-openapi.yml
- filename: morningstar-esg-api-openapi.yml
  format: yaml
  label: Morningstar Portfolio Analysis APIs
  slug: morningstar-portfolio-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-esg-api-openapi.yml
- filename: morningstar-analyst-highlights-api-openapi.yml
  format: yaml
  label: Morningstar AI Insights API
  slug: morningstar-ai-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-analyst-highlights-api-openapi.yml
- filename: morningstar-scenario-analysis-api-openapi.yml
  format: yaml
  label: Morningstar Scenario Analysis API
  slug: morningstar-scenario-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-scenario-analysis-api-openapi.yml
- filename: morningstar-clients-api-openapi.yml
  format: yaml
  label: Morningstar Risk Profiler API
  slug: morningstar-risk-profiler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-clients-api-openapi.yml
- filename: morningstar-investments-universe-api-openapi.yml
  format: yaml
  label: Morningstar Universe API
  slug: morningstar-universe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-investments-universe-api-openapi.yml
- filename: morningstar-benchmarkfees-api-openapi.yml
  format: yaml
  label: Morningstar Financial Planning APIs
  slug: morningstar-financial-planning-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-benchmarkfees-api-openapi.yml
- filename: morningstar-attribution-api-openapi.yml
  format: yaml
  label: Morningstar Investment Analysis APIs
  slug: morningstar-investment-analysis-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-attribution-api-openapi.yml
- filename: morningstar-accounts-api-openapi.yml
  format: yaml
  label: Morningstar ByAllAccounts API
  slug: morningstar-byallaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-accounts-api-openapi.yml
- filename: morningstar-morningstar-agent-api-openapi.yml
  format: yaml
  label: Morningstar Agent API
  slug: morningstar-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/openapi/morningstar-morningstar-agent-api-openapi.yml
authorization_urls:
- https://mcp.morningstar.com/authorize
description: ''
docs: https://developer.morningstar.com/direct-web-services/documentation/api-utilities/authentication-api/overview
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Morningstar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Morningstar publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Morningstar API on a user''s behalf.


  Tokens are issued from https://mcp.morningstar.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Morningstar
provider_slug: morningstar
schemes:
- flows:
  - authorizationUrl: https://mcp.morningstar.com/authorize
    dynamic_client_registration: https://mcp.morningstar.com/register
    flow: authorizationCode
    pkce: S256
    refresh_token: true
    tokenUrl: https://mcp.morningstar.com/token
  name: Morningstar MCP OAuth
  source: well-known/morningstar-oauth-authorization-server.json
scope_count: 4
scope_names:
- offline_access
- openid
- email
- profile
scopes:
- description: Refresh-token issuance for long-lived MCP client sessions.
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID-style identity scope supported by the MCP authorization server (no OIDC discovery document is published).
  flows:
  - authorizationCode
  scope: openid
- description: Access to the authenticated user's email claim.
  flows:
  - authorizationCode
  scope: email
- description: Access to the authenticated user's profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: morningstar-scopes
source_filename: morningstar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://mcp.morningstar.com/.well-known/oauth-authorization-server\ndocs: https://developer.morningstar.com/direct-web-services/documentation/api-utilities/authentication-api/overview\nschemes:\n- name: Morningstar MCP OAuth\n  source: well-known/morningstar-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.morningstar.com/authorize\n    tokenUrl: https://mcp.morningstar.com/token\n    refresh_token: true\n    pkce: S256\n    dynamic_client_registration: https://mcp.morningstar.com/register\nscopes:\n- scope: offline_access\n  description: Refresh-token issuance for long-lived MCP client sessions.\n  flows: [authorizationCode]\n  sources: [well-known/morningstar-oauth-authorization-server.json]\n- scope: openid\n  description: OpenID-style identity scope supported by the MCP authorization\n    server (no OIDC discovery document is published).\n  flows: [authorizationCode]\n\
  \  sources: [well-known/morningstar-oauth-authorization-server.json]\n- scope: email\n  description: Access to the authenticated user's email claim.\n  flows: [authorizationCode]\n  sources: [well-known/morningstar-oauth-authorization-server.json]\n- scope: profile\n  description: Access to the authenticated user's profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/morningstar-oauth-authorization-server.json]\nnotes: Direct Web Services / Dynamic Services OAuth 2.0 access tokens (POST\n  /token/oauth) are unscoped opaque bearer tokens - entitlements are bound to the\n  licensed account, not to OAuth scopes. The only published scope surface is the\n  MCP server's authorization server metadata captured above.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morningstar/refs/heads/main/scopes/morningstar-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Financial
- Market Data
- Investing
- Stocks
- Funds
- Real-Time
- Reference Data
- Portfolio Analytics
- Research
- Indexes
token_urls:
- https://mcp.morningstar.com/token
---
