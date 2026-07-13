---
api_specs:
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Programs API
  slug: boost-insurance-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Quotes API
  slug: boost-insurance-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Policies API
  slug: boost-insurance-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Claims API
  slug: boost-insurance-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Endorsements API
  slug: boost-insurance-endorsements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
- filename: boost-insurance-openapi.yml
  format: yaml
  label: Boost Insurance Webhooks API
  slug: boost-insurance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-openapi.yml
authorization_urls: []
description: ''
docs: https://learn.boostinsurance.com/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Boost Insurance Scopes
name_suffix: OAuth Scopes
note: Boost uses the OAuth 2.0 Client Credentials grant with a Client ID and Client Secret, and does not publish any OAuth scopes; access is governed by partner credentials rather than scoped tokens (https://learn.boostinsurance.com/docs/authentication).
overview: 'Boost Insurance uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.insurtech.dev/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Boost Insurance
provider_slug: boost-insurance
schemes:
- description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication endpoint and presented as a Bearer token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.insurtech.dev/auth/oauth2/token
  name: boostOAuth
  source: openapi/boost-insurance-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: boost-insurance-scopes
source_filename: boost-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/boost-insurance-openapi.yml\ndocs: https://learn.boostinsurance.com/docs/authentication\nnote: Boost uses the OAuth 2.0 Client Credentials grant with a Client ID and Client\n  Secret, and does not publish any OAuth scopes; access is governed by partner credentials\n  rather than scoped tokens (https://learn.boostinsurance.com/docs/authentication).\nschemes:\n- name: boostOAuth\n  source: openapi/boost-insurance-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.insurtech.dev/auth/oauth2/token\n  description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication\n    endpoint and presented as a Bearer token.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/scopes/boost-insurance-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Embedded Insurance
- Insurance-as-a-Service
- Policy Administration
- Claims
token_urls:
- https://api.insurtech.dev/auth/oauth2/token
---
