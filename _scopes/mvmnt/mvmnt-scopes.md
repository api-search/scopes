---
api_specs:
- filename: mvmnt-openapi-original.yml
  format: yaml
  label: MVMNT API
  slug: mvmnt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mvmnt/refs/heads/main/openapi/mvmnt-openapi-original.yml
authorization_urls: []
description: ''
docs: https://docs.mvmnt.io/getting-started/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Mvmnt Scopes
name_suffix: OAuth Scopes
note: MVMNT uses OAuth 2.0 client-credentials (machine-to-machine). The OpenAPI declares a single http bearer (JWT) scheme rather than granular oauth2 scopes. Tokens are issued with a single default scope; there is no per-resource scope taxonomy published.
overview: 'MVMNT publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the MVMNT API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MVMNT
provider_slug: mvmnt
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  tokenUrl: https://api.mvmnt.io/oauth2/token
  type: oauth2
scope_count: 1
scope_names:
- mvmnt-api
scopes:
- description: Default scope granting access to the MVMNT API surface authorized for the client.
  flows:
  - clientCredentials
  scope: mvmnt-api
slug: mvmnt-scopes
source_filename: mvmnt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.mvmnt.io/getting-started/authentication\ndocs: https://docs.mvmnt.io/getting-started/authentication\nspec_source: openapi/mvmnt-openapi-original.yml\nnote: >-\n  MVMNT uses OAuth 2.0 client-credentials (machine-to-machine). The OpenAPI declares a single\n  http bearer (JWT) scheme rather than granular oauth2 scopes. Tokens are issued with a single\n  default scope; there is no per-resource scope taxonomy published.\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    tokenUrl: https://api.mvmnt.io/oauth2/token\nscopes:\n  - scope: mvmnt-api\n    description: Default scope granting access to the MVMNT API surface authorized for the client.\n    flows: [clientCredentials]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mvmnt/refs/heads/main/scopes/mvmnt-scopes.yml
summary_line: 1 scope
tags:
- Freight
- Logistics
- Transportation Management System
- Supply Chain
- Brokerage
- Shipping
- Payments
- Company
token_urls: []
---
