---
api_specs:
- filename: s1-dev-account-api-openapi.yml
  format: yaml
  label: Search1API Account API
  slug: s1-dev-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-account-api-openapi.yml
- filename: s1-dev-crawl-api-openapi.yml
  format: yaml
  label: Search1API Crawl API
  slug: s1-dev-crawl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-crawl-api-openapi.yml
- filename: s1-dev-feedback-api-openapi.yml
  format: yaml
  label: Search1API Feedback API
  slug: s1-dev-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-feedback-api-openapi.yml
- filename: s1-dev-screenshot-api-openapi.yml
  format: yaml
  label: Search1API Screenshot API
  slug: s1-dev-screenshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-screenshot-api-openapi.yml
- filename: s1-dev-search-api-openapi.yml
  format: yaml
  label: Search1API Search API
  slug: s1-dev-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-search-api-openapi.yml
- filename: s1-dev-system-api-openapi.yml
  format: yaml
  label: Search1API System API
  slug: s1-dev-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/openapi/s1-dev-system-api-openapi.yml
authorization_urls: []
description: 'OAuth 2.1 scopes advertised by the Search1API protected-resource metadata. Access is account-scoped rather than permission-scoped: a token maps to the same user and credit balance as an API key.'
docs: https://s1.dev/auth.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: S1 Dev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Search1API publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Search1API API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Search1API
provider_slug: s1-dev
schemes: []
scope_count: 2
scope_names:
- openid
- offline_access
scopes:
- description: OpenID Connect identity of the authorizing Search1API account owner.
  flows: []
  scope: openid
- description: 'Issues a refresh token; auth.md: "a refresh token is issued only when offline_access is requested".'
  flows: []
  scope: offline_access
slug: s1-dev-scopes
source_filename: s1-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: searched\nsource: https://api.search1api.com/.well-known/oauth-protected-resource (scopes_supported); https://s1.dev/auth.md\ndocs: https://s1.dev/auth.md\ndescription: 'OAuth 2.1 scopes advertised by the Search1API protected-resource metadata. Access is account-scoped\n  rather than permission-scoped: a token maps to the same user and credit balance as an API key.'\nauthorization_server: https://clerk.s1.dev\nscopes:\n- name: openid\n  description: OpenID Connect identity of the authorizing Search1API account owner.\n- name: offline_access\n  description: 'Issues a refresh token; auth.md: \"a refresh token is issued only when offline_access is requested\".'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/s1-dev/refs/heads/main/scopes/s1-dev-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Search
- Web Search
- Crawling
- Web Scraping
- News
- AI Agents
- MCP
- Agent Tools
- Data Extraction
- Screenshots
token_bound: false
token_urls: []
---
