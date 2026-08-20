---
api_specs:
- filename: wealth-x-dossiers-api-openapi.yml
  format: yaml
  label: Wealth-X Dossiers API
  slug: wealth-x-dossiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-dossiers-api-openapi.yml
- filename: wealth-x-reference-api-openapi.yml
  format: yaml
  label: Wealth-X Reference API
  slug: wealth-x-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-reference-api-openapi.yml
- filename: wealth-x-search-api-openapi.yml
  format: yaml
  label: Wealth-X Search API
  slug: wealth-x-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/openapi/wealth-x-search-api-openapi.yml
authorization_urls: []
description: OAuth scopes for the Wealth-X / Altrata surfaces. The legacy Wealth-X Connect REST API uses three static API-key headers and declares no OAuth at all, so it has no scopes. The successor Altrata platform runs two distinct OAuth flows, and only one of them publishes a scope list anonymously.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Wealth X Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Wealth-X uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wealth-X
provider_slug: wealth-x
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: wealth-x-scopes
source_filename: wealth-x-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://mcp.altrata.com/.well-known/oauth-protected-resource\ndescription: >-\n  OAuth scopes for the Wealth-X / Altrata surfaces. The legacy Wealth-X Connect\n  REST API uses three static API-key headers and declares no OAuth at all, so it\n  has no scopes. The successor Altrata platform runs two distinct OAuth flows,\n  and only one of them publishes a scope list anonymously.\nsurfaces:\n  - name: Altrata MCP server\n    endpoint: https://mcp.altrata.com/mcp\n    flow: authorization_code + PKCE (S256)\n    authorization_server: https://mcp.altrata.com\n    authorization_endpoint: https://serviceauth.altrata.com/oauth2/authorize\n    token_endpoint: https://serviceauth.altrata.com/oauth2/token\n    scopes_published: true\n    scopes:\n      - name: openid\n        description: >-\n          OpenID Connect subject identity. Advertised in the protected-resource\n          metadata and in the WWW-Authenticate challenge on HTTP\
  \ 401.\n        source: probed\n      - name: email\n        description: >-\n          Access to the authenticated user's email claim. Advertised in the\n          protected-resource metadata and in the WWW-Authenticate challenge.\n        source: probed\n    note: >-\n      Only the two standard OIDC identity scopes are advertised. Altrata does\n      not publish resource-level scopes (per-dataset or per-tool); what a caller\n      may read is decided by their subscription entitlement, not by an OAuth\n      scope. See plans/wealth-x-plans-pricing.yml.\n  - name: Altrata GraphQL platform APIs\n    endpoint: https://api.auth.altrata.com/oauth2/token\n    flow: client_credentials\n    scopes_published: false\n    scopes: []\n    note: >-\n      docs.altrata.com/service-user-credentials documents a client_credentials\n      token request that carries an `x-api-key` header plus HTTP Basic service\n      user credentials. No `scope` parameter and no scope list are documented,\n      and the\
  \ token endpoint did not answer an anonymous probe.\n    docs: https://docs.altrata.com/service-user-credentials\n  - name: Wealth-X Connect REST API (legacy)\n    endpoint: https://connect.wealthx.com/rest/v1\n    flow: none\n    scopes_published: false\n    scopes: []\n    note: Static `username`, `password` and `apikey` request headers. No OAuth, no scopes.\nauthorization_model:\n  type: entitlement-based\n  description: >-\n    Access is governed by subscription entitlements rather than OAuth scopes.\n    Requesting a field outside the entitlement returns an error block with\n    errorType `unauthorized` while the rest of the response payload remains\n    valid and consumable.\n  source: https://docs.altrata.com/errors-warnings-and-limits\nevidence:\n  - url: https://mcp.altrata.com/.well-known/oauth-protected-resource\n    status: 200\n  - url: https://mcp.altrata.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://mcp.altrata.com/mcp\n    status: 401\n \
  \   note: 'WWW-Authenticate: Bearer realm=\"Altrata MCP\" ... scope=\"openid email\"'\n  - url: https://api.auth.altrata.com/oauth2/token\n    status: 0\n    note: No anonymous response.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealth-x/refs/heads/main/scopes/wealth-x-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Wealth Intelligence
- Data
- UHNW
- Prospecting
- Financial-Services
- CRM
- People Data
- Altrata
- GraphQL
- MCP
- Wealth Screening
token_urls: []
---
