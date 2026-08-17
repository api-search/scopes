---
api_specs:
- filename: searchapi-search-api-openapi.yml
  format: yaml
  label: SearchApi SERP API
  slug: searchapi-serp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/openapi/searchapi-search-api-openapi.yml
- filename: searchapi-account-api-openapi.yml
  format: yaml
  label: SearchApi Account & Analytics API
  slug: searchapi-account-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/openapi/searchapi-account-api-openapi.yml
authorization_urls: []
description: ''
docs: https://www.searchapi.io/integrations/mcp
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Searchapi Scopes
name_suffix: OAuth Scopes
note: 'SearchApi''s REST SERP API has no OAuth surface at all — it authenticates with a single API key (query `api_key` or `Authorization: Bearer`). The OAuth surface described here belongs exclusively to the hosted MCP server at https://www.searchapi.io/mcp, which SearchApi added alongside the legacy static `X-MCP-Token` header. The authorization server publishes exactly one scope. Scopes were read from the live RFC 8414 metadata document, not derived from a spec — `derive-oauth-scopes.py` finds no oauth2 securityScheme because the OpenAPI describes only the API-key REST surface.'
overview: 'SearchApi uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SearchApi
provider_slug: searchapi
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: searchapi-scopes
source_filename: searchapi-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://www.searchapi.io/.well-known/oauth-authorization-server\ndocs: https://www.searchapi.io/integrations/mcp\nnote: >-\n  SearchApi's REST SERP API has no OAuth surface at all — it authenticates with a\n  single API key (query `api_key` or `Authorization: Bearer`). The OAuth surface\n  described here belongs exclusively to the hosted MCP server at\n  https://www.searchapi.io/mcp, which SearchApi added alongside the legacy static\n  `X-MCP-Token` header. The authorization server publishes exactly one scope.\n  Scopes were read from the live RFC 8414 metadata document, not derived from a\n  spec — `derive-oauth-scopes.py` finds no oauth2 securityScheme because the\n  OpenAPI describes only the API-key REST surface.\nauthorization_server:\n  issuer: https://www.searchapi.io\n  metadata: https://www.searchapi.io/.well-known/oauth-authorization-server\n  authorization_endpoint: https://www.searchapi.io/oauth/authorize\n  token_endpoint:\
  \ https://www.searchapi.io/oauth/token\n  revocation_endpoint: https://www.searchapi.io/oauth/revoke\n  registration_endpoint: https://www.searchapi.io/oauth/register\n  grant_types_supported:\n    - authorization_code\n    - refresh_token\n  response_types_supported:\n    - code\n  code_challenge_methods_supported:\n    - S256\n  token_endpoint_auth_methods_supported:\n    - none\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  authorization_response_iss_parameter_supported: true\nprotected_resources:\n  - resource: https://www.searchapi.io/mcp\n    metadata: https://www.searchapi.io/.well-known/oauth-protected-resource\n    authorization_servers:\n      - https://www.searchapi.io\n    bearer_methods_supported:\n      - header\n    www_authenticate_observed: >-\n      Bearer resource_metadata=\"https://www.searchapi.io/.well-known/oauth-protected-resource/mcp\",\n      scope=\"mcp\"\nscopes:\n  - name: mcp\n    description: >-\n      Grants an OAuth\
  \ client access to the SearchApi hosted MCP server, and through it\n      to the search tools bound to the authorizing account's MCP integration. There is\n      no finer-grained scope: the single `mcp` scope carries the whole tool surface,\n      and per-tool scoping is done out-of-band by choosing which tools go into a\n      dashboard \"bundle\" rather than by OAuth scope.\n    resource: https://www.searchapi.io/mcp\n    source: https://www.searchapi.io/.well-known/oauth-authorization-server\nscope_count: 1\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searchapi/refs/heads/main/scopes/searchapi-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- search
- serp-api
- google-search
- web-scraping
- search-data
- market-intelligence
- seo
- mcp
- agent-native
token_urls: []
---
