---
api_specs:
- filename: toksta-account-api-openapi.yml
  format: yaml
  label: toksta Account API
  slug: toksta-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-account-api-openapi.yml
- filename: toksta-analysis-api-openapi.yml
  format: yaml
  label: toksta Analysis API
  slug: toksta-analysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-analysis-api-openapi.yml
- filename: toksta-campaigns-api-openapi.yml
  format: yaml
  label: toksta Campaigns API
  slug: toksta-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-campaigns-api-openapi.yml
- filename: toksta-creator-lists-api-openapi.yml
  format: yaml
  label: toksta Creator Lists API
  slug: toksta-creator-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-creator-lists-api-openapi.yml
- filename: toksta-creators-api-openapi.yml
  format: yaml
  label: toksta Creators API
  slug: toksta-creators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-creators-api-openapi.yml
- filename: toksta-enrichment-api-openapi.yml
  format: yaml
  label: toksta Enrichment API
  slug: toksta-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-enrichment-api-openapi.yml
- filename: toksta-evidence-api-openapi.yml
  format: yaml
  label: toksta Evidence API
  slug: toksta-evidence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-evidence-api-openapi.yml
- filename: toksta-jobs-api-openapi.yml
  format: yaml
  label: toksta Jobs API
  slug: toksta-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-jobs-api-openapi.yml
- filename: toksta-system-api-openapi.yml
  format: yaml
  label: toksta System API
  slug: toksta-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/openapi/toksta-system-api-openapi.yml
authorization_urls: []
description: ''
docs: https://help.toksta.com/account/managing-api-keys
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Toksta Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'toksta uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: toksta
provider_slug: toksta
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: toksta-scopes
source_filename: toksta-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://help.toksta.com/public-api/authentication\ndocs: https://help.toksta.com/account/managing-api-keys\nalso_sourced_from:\n- 'https://api.toksta.com/v1/ (live endpoint metadata, anonymous)'\n- https://help.toksta.com/public-api/getting-started\n- well-known/toksta-mcp-oauth-authorization-server.json\nmodel: api-key-endpoint-family\nsummary: >-\n  Toksta scopes access two ways, and NEITHER is an OAuth scope string. (1) An API key\n  may be restricted at creation to a subset of ENDPOINT FAMILIES; a scoped key calling\n  a disallowed route returns 403 FORBIDDEN. (2) Plan entitlement flags gate whole\n  families regardless of key scope. The MCP server's OAuth authorization server\n  publishes no scopes_supported at all — entitlement there is plan + credit balance.\noauth2:\n  present: true\n  authorization_server: https://zkdnqaotketigndjpfqw.supabase.co/auth/v1\n  applies_to: https://mcp.toksta.com/mcp\n  scopes_supported:\
  \ null\n  scopes_note: >-\n    The RFC 8414 metadata document declares no scopes_supported array, so there are no\n    OAuth scope strings to enumerate. Recorded as an honest null, not an empty guess.\n  see: authentication/toksta-authentication.yml\nendpoint_families:\n- family: data\n  description: Creator search, discovery, enrichment, fit analysis and post evidence.\n  routes:\n  - POST /v1/creators/search\n  - POST /v1/creators/discovery-search\n  - POST /v1/creators/thought-leaders\n  - GET /v1/creators/{id}\n  - POST /v1/creators/enrich\n  - POST /v1/creators/content-match\n  - POST /v1/creators/audience-match\n  - POST /v1/search-results/posts\n  - POST /v1/enrichments/results\n  - POST /v1/content-match/results\n  - POST /v1/content-match/posts\n  - POST /v1/audience-match/results\n  - POST /v1/audience-match/details\n  available_to: [dedicated-api plans, 'SaaS plans when api_access_enabled']\n- family: job\n  description: Async job status, results and cancellation.\n  routes:\n\
  \  - GET /v1/jobs/{id}\n  - POST /v1/jobs/results\n  - 'POST /v1/jobs/results:bulk'\n  - POST /v1/jobs/{id}/cancel\n  available_to: [dedicated-api plans, 'SaaS plans when api_access_enabled']\n- family: account\n  description: Metering and plan entitlement read-out.\n  routes:\n  - GET /v1/account/usage\n  available_to: [dedicated-api plans, 'SaaS plans when api_access_enabled']\n- family: workspace\n  description: Campaign and creator-list management inside a Toksta workspace.\n  routes:\n  - GET /v1/campaigns\n  - POST /v1/campaigns\n  - GET /v1/campaigns/{id}\n  - GET /v1/creator-lists\n  - POST /v1/creator-lists\n  - POST /v1/creator-lists/{id}/creators\n  available_to: ['SaaS plans when workspace_endpoints_enabled']\n  denied_to: [dedicated-api plans]\n  denial_response: 403 FORBIDDEN\nentitlement_flags:\n- flag: api_access_enabled\n  effect: Permits a SaaS plan to create API keys and call data/job/account families.\n- flag: workspace_endpoints_enabled\n  effect: Permits API access\
  \ to the workspace family.\n- flag: rate_limit_per_minute\n  effect: Sets the per-key request ceiling; default fallback 60 req/min on SaaS.\nkey_scoping:\n  supported: true\n  granularity: endpoint family\n  set_at: key creation\n  changeable: 'Not documented — rotation is the documented path to a new secret, not to new scope.'\n  violation_response: 403 FORBIDDEN\n  enumerated_scope_strings: null\n  enumerated_scope_strings_note: >-\n    The docs describe scope restriction as choosing \"which endpoint families\" a key may\n    call, but do not publish the literal scope identifiers used in the UI. The four\n    family names above come from the endpoint_family field the API itself returns on\n    GET /v1/, which is the authoritative machine-readable source.\ncross_links:\n  authentication: authentication/toksta-authentication.yml\n  conventions: conventions/toksta-conventions.yml\n  plans: plans/toksta-plans-pricing.yml\n  mcp: mcp/toksta-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toksta/refs/heads/main/scopes/toksta-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Influencer Marketing
- Marketing
- B2B
- Creator Discovery
- AI Agents
- LinkedIn
- YouTube
- Software-as-a-Service
- Creator Data
- MCP
- Brand Monitoring
token_urls: []
---
