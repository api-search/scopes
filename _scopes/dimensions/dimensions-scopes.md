---
api_specs:
- filename: dimensions-authentication-api-openapi.yml
  format: yaml
  label: Dimensions Authentication API
  slug: dimensions-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/openapi/dimensions-authentication-api-openapi.yml
- filename: dimensions-query-api-openapi.yml
  format: yaml
  label: Dimensions Query API
  slug: dimensions-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/openapi/dimensions-query-api-openapi.yml
authorization_urls: []
description: OAuth scopes Dimensions publishes. There is exactly one, and it belongs to the remote MCP endpoint on www.dimensions.ai — not to the Analytics API, which uses an unscoped API key exchanged for a JWT. Recorded because the scope surface is machine-readable and served by the provider, and because a reader looking for Dimensions OAuth scopes needs to know that the Analytics API has none.
docs: https://www.dimensions.ai/.well-known/oauth-protected-resource
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Dimensions Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Dimensions uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Dimensions
provider_slug: dimensions
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: dimensions-scopes
source_filename: dimensions-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://www.dimensions.ai/.well-known/oauth-authorization-server\ndocs: https://www.dimensions.ai/.well-known/oauth-protected-resource\nprovider: Dimensions\nproviderId: dimensions\ndescription: >-\n  OAuth scopes Dimensions publishes. There is exactly one, and it belongs to the\n  remote MCP endpoint on www.dimensions.ai — not to the Analytics API, which uses\n  an unscoped API key exchanged for a JWT. Recorded because the scope surface is\n  machine-readable and served by the provider, and because a reader looking for\n  Dimensions OAuth scopes needs to know that the Analytics API has none.\nissuer: https://www.dimensions.ai\nauthorization_endpoint: https://www.dimensions.ai/oauth/authorize\ntoken_endpoint: https://www.dimensions.ai/oauth/token\nrevocation_endpoint: https://www.dimensions.ai/oauth/revoke\nflows:\n- authorization_code\n- refresh_token\npkce: S256\nresource: https://www.dimensions.ai/wp-json/mcp/mcp-oauth-server\n\
  scope_count: 1\nscopes:\n- name: mcp\n  description: >-\n    The single scope advertised by both the authorization-server metadata\n    (scopes_supported) and the protected-resource metadata. It grants access to\n    the site's MCP endpoint. No finer-grained read/write split is published, and\n    no per-tool scope mapping is discoverable anonymously.\n  source: https://www.dimensions.ai/.well-known/oauth-authorization-server\nnot_applicable:\n  surface: Dimensions Analytics API\n  reason: >-\n    Authentication is an API key exchanged for a JWT. The published OpenAPI\n    declares an apiKey securityScheme and no oauth2 flows, and the docs describe\n    no permission or scope model — entitlements are carried by the institutional\n    subscription attached to the key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dimensions/refs/heads/main/scopes/dimensions-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Analytics
- Research
- Publications
- Grants
- Patents
- Clinical Trials
- Jupyter Notebooks
- Scientometrics
- Bibliometrics
- Research Intelligence
- Datasets
- Policy Documents
- MCP
token_urls: []
---
