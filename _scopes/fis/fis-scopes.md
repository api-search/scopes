---
api_specs:
- filename: fis-accounts-api-openapi.yml
  format: yaml
  label: FIS Global Accounts API
  slug: fis-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-accounts-api-openapi.yml
- filename: fis-ach-api-openapi.yml
  format: yaml
  label: FIS Global ACH API
  slug: fis-ach-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-ach-api-openapi.yml
- filename: fis-payments-api-openapi.yml
  format: yaml
  label: FIS Global Payments API
  slug: fis-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-payments-api-openapi.yml
- filename: fis-transactions-api-openapi.yml
  format: yaml
  label: FIS Global Transactions API
  slug: fis-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-transactions-api-openapi.yml
- filename: fis-wire-transfers-api-openapi.yml
  format: yaml
  label: FIS Global Wire Transfers API
  slug: fis-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/fis-wire-transfers-api-openapi.yml
- filename: fis-accounting-data-as-a-service-openapi.json
  format: json
  label: FIS Accounting Data as a Service
  slug: fis-accounting-data-as-a-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/openapi/_original/fis-accounting-data-as-a-service-openapi.json
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Fis Scopes
name_suffix: OAuth Scopes
note: FIS publishes no OAuth scope surface that a member of the public can read. The one public contract, FIS Accounting Data as a Service, authenticates with an opaque bearer token minted from a Basic-auth key pair — it declares no oauth2 securityScheme and no scopes, so there is nothing to enumerate. FIS Code Connect generates client keys behind a reviewed registration; whatever scope model it uses is not visible without an account.
overview: 'FIS Global uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FIS Global
provider_slug: fis
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: fis-scopes
source_filename: fis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: searched\nsource: https://docs.railz.ai/reference/authentication + openapi/_original/fis-accounting-data-as-a-service-openapi.json\nscope_count: 0\nschemes: []\nscopes: []\nnote: >-\n  FIS publishes no OAuth scope surface that a member of the public can read. The one public\n  contract, FIS Accounting Data as a Service, authenticates with an opaque bearer token minted\n  from a Basic-auth key pair — it declares no oauth2 securityScheme and no scopes, so there is\n  nothing to enumerate. FIS Code Connect generates client keys behind a reviewed registration;\n  whatever scope model it uses is not visible without an account.\nsupersedes:\n  note: >-\n    Replaces the 2026-07-11 derived file, which listed accounts:read / payments:read /\n    payments:write against a tokenUrl of https://api.fisglobal.com/oauth/token. That host\n    returns NXDOMAIN and no FIS document reachable without a Code Connect account corroborates\n    those scope names, so\
  \ they are withdrawn rather than carried forward. The OAuthScopes\n    pointer is withdrawn from apis.yml with them — an empty scope surface should not be\n    credited as a documented one.\nevidence:\n- url: https://api.railz.ai/swagger.json\n  status: 200\n  detail: 'securitySchemes contains only a bearer entry of type http, scheme bearer; no oauth2 flow and no scopes map.'\n- url: https://codeconnect.fisglobal.com/app/guides/authenticate\n  status: 200\n  detail: 200 returns the Angular application shell; the guide body renders only after login.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fis/refs/heads/main/scopes/fis-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Banking
- Core Banking
- Financial-Services
- Payments
- Fintech
token_urls: []
---
