---
api_specs:
- filename: nordic-financial-news-articles-api-openapi.yml
  format: yaml
  label: Nordic Financial News Articles API
  slug: nordic-financial-news-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-articles-api-openapi.yml
- filename: nordic-financial-news-calendar-events-api-openapi.yml
  format: yaml
  label: Nordic Financial News Calendar Events API
  slug: nordic-financial-news-calendar-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-calendar-events-api-openapi.yml
- filename: nordic-financial-news-categories-api-openapi.yml
  format: yaml
  label: Nordic Financial News Categories API
  slug: nordic-financial-news-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-categories-api-openapi.yml
- filename: nordic-financial-news-companies-api-openapi.yml
  format: yaml
  label: Nordic Financial News Companies API
  slug: nordic-financial-news-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-companies-api-openapi.yml
- filename: nordic-financial-news-countries-api-openapi.yml
  format: yaml
  label: Nordic Financial News Countries API
  slug: nordic-financial-news-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-countries-api-openapi.yml
- filename: nordic-financial-news-event-types-api-openapi.yml
  format: yaml
  label: Nordic Financial News Event Types API
  slug: nordic-financial-news-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-event-types-api-openapi.yml
- filename: nordic-financial-news-events-api-openapi.yml
  format: yaml
  label: Nordic Financial News Events API
  slug: nordic-financial-news-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-events-api-openapi.yml
- filename: nordic-financial-news-exchanges-api-openapi.yml
  format: yaml
  label: Nordic Financial News Exchanges API
  slug: nordic-financial-news-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-exchanges-api-openapi.yml
- filename: nordic-financial-news-health-api-openapi.yml
  format: yaml
  label: Nordic Financial News Health API
  slug: nordic-financial-news-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-health-api-openapi.yml
- filename: nordic-financial-news-indices-api-openapi.yml
  format: yaml
  label: Nordic Financial News Indices API
  slug: nordic-financial-news-indices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-indices-api-openapi.yml
- filename: nordic-financial-news-meta-api-openapi.yml
  format: yaml
  label: Nordic Financial News Meta API
  slug: nordic-financial-news-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-meta-api-openapi.yml
- filename: nordic-financial-news-search-api-openapi.yml
  format: yaml
  label: Nordic Financial News Search API
  slug: nordic-financial-news-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-search-api-openapi.yml
- filename: nordic-financial-news-sources-api-openapi.yml
  format: yaml
  label: Nordic Financial News Sources API
  slug: nordic-financial-news-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-sources-api-openapi.yml
- filename: nordic-financial-news-stories-api-openapi.yml
  format: yaml
  label: Nordic Financial News Stories API
  slug: nordic-financial-news-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-stories-api-openapi.yml
- filename: nordic-financial-news-watchlists-api-openapi.yml
  format: yaml
  label: Nordic Financial News Watchlists API
  slug: nordic-financial-news-watchlists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/openapi/nordic-financial-news-watchlists-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.nordicfinancialnews.com/guides/authentication.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Nordic Financial News Scopes
name_suffix: OAuth Scopes
note: Scopes apply to API keys and to MCP OAuth connections; all scopes are enabled by default.
overview: 'Nordic Financial News publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Nordic Financial News API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nordic Financial News
provider_slug: nordic-financial-news
schemes: []
scope_count: 2
scope_names:
- read
- read:watchlist
scopes:
- description: All content (articles, stories, companies, categories, countries, exchanges, indices, sources, search)
  flows: []
  scope: read
- description: Read your watchlists and their companies
  flows: []
  scope: read:watchlist
slug: nordic-financial-news-scopes
source_filename: nordic-financial-news-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "name: Nordic Financial News API key scopes\ngenerated: '2026-10-09'\nmethod: searched\nsource: https://docs.nordicfinancialnews.com/guides/authentication.md\ndocs: https://docs.nordicfinancialnews.com/guides/authentication.md\nnote: Scopes apply to API keys and to MCP OAuth connections; all scopes are enabled by default.\nscopes:\n- name: read\n  description: All content (articles, stories, companies, categories, countries, exchanges, indices, sources, search)\n- name: read:watchlist\n  description: Read your watchlists and their companies\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nordic-financial-news/refs/heads/main/scopes/nordic-financial-news-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Financial News
- Nordic
- Market Data
- Financial Calendar
- MCP
- News API
token_bound: false
token_urls: []
---
