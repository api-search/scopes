---
api_specs:
- filename: chathome-lu-agent-api-openapi.yml
  format: yaml
  label: ChatHome Protected Agent API
  slug: protected-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-agent-api-openapi.yml
- filename: chathome-lu-agents-api-openapi.yml
  format: yaml
  label: ChatHome Agents API
  slug: chathome-lu-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-agents-api-openapi.yml
- filename: chathome-lu-listings-api-openapi.yml
  format: yaml
  label: ChatHome Listings API
  slug: chathome-lu-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-listings-api-openapi.yml
- filename: chathome-lu-market-data-api-openapi.yml
  format: yaml
  label: ChatHome Market data API
  slug: chathome-lu-market-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-market-data-api-openapi.yml
- filename: chathome-lu-search-api-openapi.yml
  format: yaml
  label: ChatHome Search API
  slug: chathome-lu-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chathome-lu/openapi/chathome-lu-search-api-openapi.yml
authorization_urls: []
description: ''
docs: https://chathome.lu/en/developers
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: ChatHome Scopes
name_suffix: OAuth Scopes
note: Scopes are not declared in the OpenAPI (the agent API uses an http bearer scheme); they are published in the developer portal, llms.txt and the authorization-server metadata scopes_supported (GET 200 on 2026-11-03).
overview: 'ChatHome publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the ChatHome API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ChatHome
provider_slug: chathome-lu
schemes: []
scope_count: 5
scope_names:
- listings:read
- market:read
- documents:write
- inquiries:write
- inquiries:read
scopes:
- description: Read listing access for search, interactive cards, get_listing, and get_listing_truth.
  flows: []
  scope: listings:read
- description: Read market access for context, valuation, affordability, and commute tools. Required by POST /api/agent/v1/estimates (getPropertyEstimateReport) when using a bearer token.
  flows: []
  scope: market:read
- description: Write access to persist a private analysis of a user-provided lease. Required for analyze_lease.
  flows: []
  scope: documents:write
- description: Write access to create inquiry conversations on behalf of the authenticated user. Required for submit_inquiry.
  flows: []
  scope: inquiries:write
- description: Read access to inquiry conversations created by this API key. Required for get_inquiry_status.
  flows: []
  scope: inquiries:read
slug: chathome-lu-scopes
source_filename: chathome-lu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://chathome.lu/en/developers\ndocs: https://chathome.lu/en/developers\nmetadata: https://chathome.lu/.well-known/oauth-authorization-server\nnote: Scopes are not declared in the OpenAPI (the agent API uses an http bearer scheme); they are published in the developer portal, llms.txt and the authorization-server metadata scopes_supported (GET 200 on 2026-11-03).\nscopes:\n- name: listings:read\n  description: Read listing access for search, interactive cards, get_listing, and get_listing_truth.\n- name: market:read\n  description: Read market access for context, valuation, affordability, and commute tools. Required by POST /api/agent/v1/estimates (getPropertyEstimateReport) when using a bearer token.\n  operations:\n  - getPropertyEstimateReport\n- name: documents:write\n  description: Write access to persist a private analysis of a user-provided lease. Required for analyze_lease.\n- name: inquiries:write\n  description:\
  \ Write access to create inquiry conversations on behalf of the authenticated user. Required for submit_inquiry.\n- name: inquiries:read\n  description: Read access to inquiry conversations created by this API key. Required for get_inquiry_status.\n"
source_yaml_url: https://artifacts.apis.io/chathome-lu/scopes/chathome-lu-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Real Estate
- Property Search
- Luxembourg
- Housing
- Property Valuation
- AI Agents
- MCP
- A2A
token_bound: false
token_urls: []
---
