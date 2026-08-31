---
api_specs:
- filename: algolia-search-api-openapi.yml
  format: yaml
  label: Algolia Search API
  slug: algolia-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-search-api-openapi.yml
- filename: algolia-insights-api-openapi.yml
  format: yaml
  label: Algolia Insights API
  slug: algolia-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-insights-api-openapi.yml
- filename: algolia-recommend-api-openapi.yml
  format: yaml
  label: Algolia Recommend API
  slug: algolia-recommend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-recommend-api-openapi.yml
- filename: algolia-analytics-api-openapi.yml
  format: yaml
  label: Algolia Analytics API
  slug: algolia-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-analytics-api-openapi.yml
- filename: algolia-abtesting-v3-api-openapi.yml
  format: yaml
  label: Algolia A/B Testing API
  slug: algolia-ab-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-abtesting-v3-api-openapi.yml
- filename: algolia-personalization-api-openapi.yml
  format: yaml
  label: Algolia Personalization API
  slug: algolia-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-personalization-api-openapi.yml
- filename: algolia-advanced-personalization-api-openapi.yml
  format: yaml
  label: Algolia Advanced Personalization API
  slug: algolia-advanced-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-advanced-personalization-api-openapi.yml
- filename: algolia-crawler-api-openapi.yml
  format: yaml
  label: Algolia Crawler API
  slug: algolia-crawler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-crawler-api-openapi.yml
- filename: algolia-ingestion-api-openapi.yml
  format: yaml
  label: Algolia Ingestion API
  slug: algolia-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-ingestion-api-openapi.yml
- filename: algolia-query-suggestions-api-openapi.yml
  format: yaml
  label: Algolia Query Suggestions API
  slug: algolia-query-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-query-suggestions-api-openapi.yml
- filename: algolia-composition-api-openapi.yml
  format: yaml
  label: Algolia Composition API
  slug: algolia-composition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-composition-api-openapi.yml
- filename: algolia-agent-studio-api-openapi.yml
  format: yaml
  label: Algolia Agent Studio API
  slug: algolia-agent-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-agent-studio-api-openapi.yml
- filename: algolia-monitoring-api-openapi.yml
  format: yaml
  label: Algolia Monitoring API
  slug: algolia-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/openapi/algolia-monitoring-api-openapi.yml
authorization_urls: []
description: 'Algolia''s REST APIs do NOT use OAuth - all 15 first-party OpenAPI documents declare apiKey-in-header (x-algolia-application-id + x-algolia-api-key) or, for the Crawler, HTTP Basic. Running derive-oauth-scopes.py over openapi/ finds zero oauth2 securitySchemes, correctly. OAuth exists in exactly one place in the estate: the Algolia Productivity MCP server. Its scope set was read from the RFC 9728 protected-resource metadata document, not inferred.'
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Algolia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Algolia uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Algolia
provider_slug: algolia
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: algolia-scopes
source_filename: algolia-scopes.yml
source_heading: OAuth Scopes
source_url: https://mcp.algolia.com/.well-known/oauth-protected-resource
source_yaml: "specification: API Commons OAuth Scopes\nspecificationVersion: '0.1'\nprovider: Algolia\nproviderId: algolia\ngenerated: '2026-08-27'\nmethod: probed\nsource: https://mcp.algolia.com/.well-known/oauth-protected-resource\nsources:\n  - https://mcp.algolia.com/.well-known/oauth-protected-resource\n  - https://mcp.algolia.com/.well-known/oauth-authorization-server\n  - https://www.algolia.com/doc/guides/model-context-protocol/productivity-mcp\n  - https://www.algolia.com/doc/guides/security/api-keys/in-depth/api-key-restrictions\ndescription: >-\n  Algolia's REST APIs do NOT use OAuth - all 15 first-party OpenAPI documents declare apiKey-in-header\n  (x-algolia-application-id + x-algolia-api-key) or, for the Crawler, HTTP Basic. Running\n  derive-oauth-scopes.py over openapi/ finds zero oauth2 securitySchemes, correctly.\n  OAuth exists in exactly one place in the estate: the Algolia Productivity MCP server. Its scope set was read\n  from the RFC 9728 protected-resource metadata\
  \ document, not inferred.\nrest_oauth: false\nrest_auth_model: api-key-with-acl\noauth_surfaces:\n  - name: Algolia Productivity MCP\n    resource: https://mcp.algolia.com/mcp\n    issuer: https://dashboard.algolia.com\n    authorization_endpoint: https://dashboard.algolia.com/2/oauth/authorize\n    token_endpoint: https://dashboard.algolia.com/2/oauth/token\n    registration_endpoint: https://dashboard.algolia.com/2/oauth/register\n    introspection_endpoint: https://dashboard.algolia.com/2/oauth/introspect\n    revocation_endpoint: https://dashboard.algolia.com/2/oauth/token\n    grant_types: [authorization_code, refresh_token]\n    response_types: [code]\n    pkce_methods: [S256]\n    client_auth_methods: [none]\n    dynamic_registration: true\n    scopes:\n      - name: public\n        description: >-\n          The only scope Algolia advertises for the MCP resource. It is coarse by design: authorization is NOT\n          carried by the scope but by the signed-in user's own Algolia\
  \ permissions, which decide which applications\n          and indices the agent can reach. A single scope string therefore expands to a different effective\n          permission set per user.\n        source: 'scopes_supported in https://mcp.algolia.com/.well-known/oauth-protected-resource'\n    probe:\n      url: https://mcp.algolia.com/mcp\n      http_status: 401\n      www_authenticate: 'Bearer resource_metadata=\"https://mcp.algolia.com/.well-known/oauth-protected-resource\", scope=\"public\"'\neffective_authorization_model:\n  note: >-\n    Where a scope string would normally sit, Algolia puts an ACL on the API key. This is the real permission\n    vocabulary for the REST surface and every operation reference names the ACL it requires.\n  mechanism: api-key-acl\n  docs: https://www.algolia.com/doc/guides/security/api-keys/in-depth/api-key-restrictions\n  acls:\n    - search\n    - browse\n    - addObject\n    - deleteObject\n    - deleteIndex\n    - settings\n    - editSettings\n\
  \    - analytics\n    - recommendation\n    - usage\n    - logs\n    - seeUnretrievableAttributes\n    - listIndexes\n  acl_source: >-\n    Enumerated from the ACL values documented on the API key restrictions page and used across the Search API\n    operation reference. Not read from a machine-readable enum - Algolia does not publish the ACL list as one.\n  restrictions:\n    - validUntil (expiry)\n    - restrictIndices\n    - restrictSources (IP)\n    - referers\n    - maxQueriesPerIPPerHour\n    - maxHitsPerQuery\n  secured_api_keys:\n    note: >-\n      A search-only key can be signed client-side with embedded filters to produce a per-end-user key, which is\n      Algolia's answer to per-tenant authorization without an authorization server.\n    docs: https://www.algolia.com/doc/guides/security/api-keys/how-to/user-restricted-access-to-data\n  limit: 5,000 API keys per application (documented service limit).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algolia/refs/heads/main/scopes/algolia-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Search
- Discovery
- Recommendations
- Personalization
- Analytics
- E-Commerce
token_urls: []
---
