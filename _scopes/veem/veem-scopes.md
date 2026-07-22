---
api_specs:
- filename: veem-api-openapi.yml
  format: yaml
  label: Veem Public API
  slug: veem-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-api-openapi.yml
authorization_urls:
- https://api.veem.com/oauth/authorize
description: OAuth scope surface for the Veem Public API. Veem documents a single coarse-grained scope, "all", used across both the two-legged (client_credentials) and three-legged (authorization_code) flows — there is no published per-resource scope or permission catalog. The published OpenAPI slices declare no oauth2 securitySchemes, so the mechanical derive pass found no in-spec scopes; this file is sourced from the OAuth guide.
docs: https://developer.veem.com/docs/oauth
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Veem Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Veem publishes 1 OAuth 2.0 scope via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Veem API on a user''s behalf.


  Tokens are issued from https://api.veem.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Veem
provider_slug: veem
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.veem.com/oauth/token
  - authorizationUrl: https://api.veem.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.veem.com/oauth/token
  name: OAuth2
  source: https://developer.veem.com/docs/oauth
scope_count: 1
scope_names:
- all
scopes:
- description: Full access to the Veem Public API on behalf of the authorized account; the only scope Veem documents.
  flows:
  - clientCredentials
  - authorizationCode
  scope: all
slug: veem-scopes
source_filename: veem-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.veem.com/docs/oauth\ndocs: https://developer.veem.com/docs/oauth\ndescription: >-\n  OAuth scope surface for the Veem Public API. Veem documents a single\n  coarse-grained scope, \"all\", used across both the two-legged\n  (client_credentials) and three-legged (authorization_code) flows — there is\n  no published per-resource scope or permission catalog. The published OpenAPI\n  slices declare no oauth2 securitySchemes, so the mechanical derive pass found\n  no in-spec scopes; this file is sourced from the OAuth guide.\nschemes:\n  - name: OAuth2\n    source: https://developer.veem.com/docs/oauth\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://api.veem.com/oauth/token\n      - flow: authorizationCode\n        authorizationUrl: https://api.veem.com/oauth/authorize\n        tokenUrl: https://api.veem.com/oauth/token\nscopes:\n  - scope: all\n    description: Full access to the Veem Public\
  \ API on behalf of the authorized account; the only scope Veem documents.\n    flows: [clientCredentials, authorizationCode]\n    sources: [https://developer.veem.com/docs/oauth]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/scopes/veem-scopes.yml
summary_line: 1 scope · clientCredentials/authorizationCode
tags:
- Payments
- B2B Payments
- Cross-Border Payments
- Invoicing
- Wallets
- Fintech
- Global Payments
token_urls:
- https://api.veem.com/oauth/token
---
