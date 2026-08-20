---
api_specs:
- filename: dataforseo-aioptimization-api-openapi.yml
  format: yaml
  label: DataForSEO AiOptimization API
  slug: dataforseo-aioptimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-aioptimization-api-openapi.yml
- filename: dataforseo-appdata-api-openapi.yml
  format: yaml
  label: DataForSEO AppData API
  slug: dataforseo-appdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-appdata-api-openapi.yml
- filename: dataforseo-appendix-api-openapi.yml
  format: yaml
  label: DataForSEO Appendix API
  slug: dataforseo-appendix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-appendix-api-openapi.yml
- filename: dataforseo-backlinks-api-openapi.yml
  format: yaml
  label: DataForSEO Backlinks API
  slug: dataforseo-backlinks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-backlinks-api-openapi.yml
- filename: dataforseo-businessdata-api-openapi.yml
  format: yaml
  label: DataForSEO BusinessData API
  slug: dataforseo-businessdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-businessdata-api-openapi.yml
- filename: dataforseo-contentanalysis-api-openapi.yml
  format: yaml
  label: DataForSEO ContentAnalysis API
  slug: dataforseo-contentanalysis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-contentanalysis-api-openapi.yml
- filename: dataforseo-dataforseolabs-api-openapi.yml
  format: yaml
  label: DataForSEO DataforseoLabs API
  slug: dataforseo-dataforseolabs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-dataforseolabs-api-openapi.yml
- filename: dataforseo-domainanalytics-api-openapi.yml
  format: yaml
  label: DataForSEO DomainAnalytics API
  slug: dataforseo-domainanalytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-domainanalytics-api-openapi.yml
- filename: dataforseo-keywordsdata-api-openapi.yml
  format: yaml
  label: DataForSEO KeywordsData API
  slug: dataforseo-keywordsdata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-keywordsdata-api-openapi.yml
- filename: dataforseo-merchant-api-openapi.yml
  format: yaml
  label: DataForSEO Merchant API
  slug: dataforseo-merchant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-merchant-api-openapi.yml
- filename: dataforseo-onpage-api-openapi.yml
  format: yaml
  label: DataForSEO OnPage API
  slug: dataforseo-onpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-onpage-api-openapi.yml
- filename: dataforseo-serp-api-openapi.yml
  format: yaml
  label: DataForSEO Serp API
  slug: dataforseo-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/openapi/dataforseo-serp-api-openapi.yml
authorization_urls:
- https://data.dataforseo.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Dataforseo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'DataForSEO publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the DataForSEO API on a user''s behalf.


  Tokens are issued from https://data.dataforseo.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: DataForSEO
provider_slug: dataforseo
schemes:
- dynamic_client_registration: true
  dynamic_client_registration_spec: RFC 7591
  flows:
  - authorizationUrl: https://data.dataforseo.com/oauth/authorize
    flow: authorizationCode
    refresh: true
    tokenUrl: https://data.dataforseo.com/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://data.dataforseo.com
  name: oauth2
  pkce_methods:
  - S256
  registration_endpoint: https://data.dataforseo.com/oauth/clients/register
  response_types:
  - code
  revocation_endpoint: https://data.dataforseo.com/oauth/tokens/revoke
  source: https://data.dataforseo.com/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
scope_count: 2
scope_names:
- api
- profile
scopes:
- description: Access to the DataForSEO API through the authorized surface. Advertised in `scopes_supported`; no further definition is published, so the exact privilege boundary is not documented.
  flows:
  - authorizationCode
  scope: api
- description: Access to the authenticated user's account profile. Advertised in `scopes_supported`; no further definition is published.
  flows:
  - authorizationCode
  scope: profile
slug: dataforseo-scopes
source_filename: dataforseo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://data.dataforseo.com/.well-known/oauth-authorization-server\ndocs: null\ndocs_note: >-\n  DataForSEO publishes no scopes/permissions reference page. The scope set below\n  was read from the live RFC 8414 authorization-server metadata document, not\n  from documentation. The MCP server README describes OAuth as \"works out of the\n  box\" and never names a scope.\n\napplies_to:\n  surface: MCP\n  resource: https://mcp.dataforseo.com\n  note: >-\n    OAuth 2.0 applies ONLY to the hosted MCP server. The v3 REST API at\n    api.dataforseo.com is HTTP Basic only and has no OAuth surface and no\n    scopes — the 12 OpenAPI documents in openapi/ declare a single `basicAuth`\n    securityScheme and nothing else.\n\nschemes:\n  - name: oauth2\n    source: https://data.dataforseo.com/.well-known/oauth-authorization-server\n    issuer: https://data.dataforseo.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl:\
  \ https://data.dataforseo.com/oauth/authorize\n        tokenUrl: https://data.dataforseo.com/oauth/token\n        refresh: true\n    pkce_methods: [S256]\n    response_types: [code]\n    grant_types: [authorization_code, refresh_token]\n    token_endpoint_auth_methods: [none]\n    registration_endpoint: https://data.dataforseo.com/oauth/clients/register\n    revocation_endpoint: https://data.dataforseo.com/oauth/tokens/revoke\n    dynamic_client_registration: true\n    dynamic_client_registration_spec: RFC 7591\n\nscopes:\n  - scope: api\n    description: >-\n      Access to the DataForSEO API through the authorized surface. Advertised in\n      `scopes_supported`; no further definition is published, so the exact\n      privilege boundary is not documented.\n    flows: [authorizationCode]\n    sources: [https://data.dataforseo.com/.well-known/oauth-authorization-server]\n  - scope: profile\n    description: >-\n      Access to the authenticated user's account profile. Advertised in\n \
  \     `scopes_supported`; no further definition is published.\n    flows: [authorizationCode]\n    sources: [https://data.dataforseo.com/.well-known/oauth-authorization-server]\n\nprotected_resource:\n  spec: RFC 9728\n  metadata:\n    - url: https://mcp.dataforseo.com/.well-known/oauth-protected-resource\n      resource: https://mcp.dataforseo.com\n    - url: https://mcp.dataforseo.com/.well-known/oauth-protected-resource/mcp\n      resource: https://mcp.dataforseo.com/mcp\n  authorization_servers: [https://data.dataforseo.com]\n  bearer_methods_supported: [header]\n\ngranularity_note: >-\n  Two coarse scopes for an API with 554 operations spanning SERP scraping,\n  keyword data, backlinks, on-page crawling and paid AI-optimization endpoints.\n  A token bearing `api` can spend account balance on any of them; there is no\n  read-only scope, no per-product scope and no spend-bounded scope. An agent\n  operator should rely on the account-level cost limits and IP whitelisting in\n  the DataForSEO\
  \ dashboard (status codes 40203 and 40207) rather than on scope\n  restriction.\n\nx-evidence:\n  fetched: '2026-08-13'\n  url: https://data.dataforseo.com/.well-known/oauth-authorization-server\n  http_status: 200\n  content_type: application/json\n  file: well-known/dataforseo-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dataforseo/refs/heads/main/scopes/dataforseo-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- SEO
- SERP
- Keywords
- Backlinks
- Domain Analytics
- On-Page SEO
- Competitor Research
- Search Engines
- Content Analysis
- E-Commerce
- App Store
- Business Data
- AI Optimization
- Social-Media
token_urls:
- https://data.dataforseo.com/oauth/token
---
