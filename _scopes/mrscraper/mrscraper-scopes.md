---
api_specs:
- filename: mrscraper-analytic-api-openapi.yml
  format: yaml
  label: MrScraper Analytic API
  slug: mrscraper-analytic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-analytic-api-openapi.yml
- filename: mrscraper-auth-api-openapi.yml
  format: yaml
  label: MrScraper Auth API
  slug: mrscraper-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-auth-api-openapi.yml
- filename: mrscraper-gateway-api-openapi.yml
  format: yaml
  label: MrScraper Gateway API
  slug: mrscraper-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-gateway-api-openapi.yml
- filename: mrscraper-jobs-api-openapi.yml
  format: yaml
  label: MrScraper Jobs API
  slug: mrscraper-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-jobs-api-openapi.yml
- filename: mrscraper-proxies-api-openapi.yml
  format: yaml
  label: MrScraper Proxies API
  slug: mrscraper-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-proxies-api-openapi.yml
- filename: mrscraper-results-api-openapi.yml
  format: yaml
  label: MrScraper Results API
  slug: mrscraper-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-results-api-openapi.yml
- filename: mrscraper-storage-api-openapi.yml
  format: yaml
  label: MrScraper Storage API
  slug: mrscraper-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-storage-api-openapi.yml
- filename: mrscraper-tasks-api-openapi.yml
  format: yaml
  label: MrScraper Tasks API
  slug: mrscraper-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/openapi/mrscraper-tasks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.mrscraper.com/docs/getting-started/mcp-server
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Mrscraper Scopes
name_suffix: OAuth Scopes
note: Scopes are issued by the OAuth 2.1 authorization server at https://api.app.mrscraper.com for the MCP resource https://mcp.mrscraper.com/mcp (RFC 9728 protected-resource metadata lists scrape:read, scrape:write, account:read; the AS metadata adds offline_access). Tool-to-scope binding is from the server source (src/scopes.ts). The REST API itself uses API tokens, not scopes.
overview: 'MrScraper publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the MrScraper API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MrScraper
provider_slug: mrscraper
schemes: []
scope_count: 4
scope_names:
- scrape:read
- scrape:write
- account:read
- offline_access
scopes:
- description: Read-only scraping and retrieval - fetch a page through the Web Renderer, run a Google SERP query, list and read stored results.
  flows: []
  scope: scrape:read
- description: Create and run scrapers - AI extraction runs and reruns of saved AI or manual scrapers.
  flows: []
  scope: scrape:write
- description: Read subscription status, quota, token usage and per-domain request outcomes.
  flows: []
  scope: account:read
- description: Issue a refresh token (listed in the authorization-server metadata scopes_supported; not bound to a tool).
  flows: []
  scope: offline_access
slug: mrscraper-scopes
source_filename: mrscraper-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: https://api.app.mrscraper.com/.well-known/oauth-authorization-server\ndocs: https://docs.mrscraper.com/docs/getting-started/mcp-server\nnote: Scopes are issued by the OAuth 2.1 authorization server at https://api.app.mrscraper.com for the MCP resource https://mcp.mrscraper.com/mcp (RFC 9728 protected-resource metadata lists scrape:read, scrape:write, account:read; the AS metadata adds offline_access). Tool-to-scope binding is from the server source (src/scopes.ts). The REST API itself uses API tokens, not scopes.\nauthorization_server:\n  issuer: https://api.app.mrscraper.com\n  authorization_endpoint: https://api.app.mrscraper.com/oauth/authorize\n  token_endpoint: https://api.app.mrscraper.com/oauth/token\n  registration_endpoint: https://api.app.mrscraper.com/oauth/register\n  revocation_endpoint: https://api.app.mrscraper.com/oauth/revoke\n  grant_types: [authorization_code, refresh_token]\n  code_challenge_methods: [S256]\n\
  scopes:\n- scope: scrape:read\n  description: Read-only scraping and retrieval - fetch a page through the Web Renderer, run a Google SERP query, list and read stored results.\n  tools: [fetch, serp, results, result]\n- scope: scrape:write\n  description: Create and run scrapers - AI extraction runs and reruns of saved AI or manual scrapers.\n  tools: [scrape, rerun]\n- scope: account:read\n  description: Read subscription status, quota, token usage and per-domain request outcomes.\n  tools: [status]\n- scope: offline_access\n  description: Issue a refresh token (listed in the authorization-server metadata scopes_supported; not bound to a tool).\n  tools: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mrscraper/refs/heads/main/scopes/mrscraper-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Web Scraping
- Data Extraction
- Proxies
- AI Agents
- MCP
- Search
- Browser Automation
token_bound: false
token_urls: []
---
