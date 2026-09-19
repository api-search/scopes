---
api_specs:
- filename: apilayer-endpoints-api-openapi.yml
  format: yaml
  label: APILayer Endpoints API
  slug: apilayer-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apilayer/refs/heads/main/openapi/apilayer-endpoints-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Apilayer Scopes
name_suffix: OAuth Scopes
note: APILayer publishes no scopes reference page. This list is read verbatim from the OAuth authorization server metadata and the MCP protected-resource descriptor, which are the only places APILayer states its scopes. Scopes apply ONLY to the hosted MCP server; the REST product APIs use an unscoped account-wide access_key.
overview: 'APILayer uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: APILayer
provider_slug: apilayer
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: apilayer-scopes
source_filename: apilayer-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: https://auth.apilayer.com/.well-known/openid-configuration and\n  https://mcp.apilayer.com/.well-known/oauth-protected-resource\nprovider: APILayer\nproviderId: apilayer\nnote: >-\n  APILayer publishes no scopes reference page. This list is read verbatim from the OAuth\n  authorization server metadata and the MCP protected-resource descriptor, which are the only\n  places APILayer states its scopes. Scopes apply ONLY to the hosted MCP server; the REST\n  product APIs use an unscoped account-wide access_key.\nauthorization_server: https://auth.apilayer.com\nprotected_resource: https://mcp.apilayer.com/mcp\nscopes:\n  - name: openid\n    description: Standard OpenID Connect scope; requests an ID token.\n    source: authorization server metadata\n  - name: offline_access\n    description: Standard OAuth scope; requests a refresh token.\n    source: authorization server metadata\n  - name: offline\n    description: Legacy alias for\
  \ offline_access advertised alongside it.\n    source: authorization server metadata\n  - name: mcp:read\n    description: Read access to the APILayer hosted MCP server.\n    source: authorization server metadata and MCP protected-resource metadata\n  - name: api:ipstack\n    description: Access to the IPstack product through the MCP server.\n    source: authorization server metadata and MCP protected-resource metadata\nfinding: >-\n  The scope list is the strongest available evidence of how much of the marketplace the MCP\n  server actually fronts. Exactly ONE product scope exists - api:ipstack - against a catalog of\n  22 published OpenAPI documents. The MCP surface is an IPstack pilot, not a marketplace-wide\n  agent door.\ndocs: null\nchecked: '2026-09-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apilayer/refs/heads/main/scopes/apilayer-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- API Marketplace
- API Catalog
- API Discovery
- Developer Tools
- SaaS APIs
- Geolocation
- Currency
- Data API
token_urls: []
---
