---
api_specs:
- filename: tackle-api-openapi.json
  format: json
  label: Tackle API
  slug: tackle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-api-openapi.json
- filename: tackle-cosell-openapi.json
  format: json
  label: Tackle Co-Sell for AWS Partner Central
  slug: tackle-co-sell-for-aws-partner-central
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-cosell-openapi.json
- filename: tackle-marketplace-openapi.json
  format: json
  label: Tackle Offers (AWS Marketplace)
  slug: tackle-offers-aws-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-marketplace-openapi.json
- filename: tackle-offers-openapi.json
  format: json
  label: Tackle Offers (Microsoft Marketplace)
  slug: tackle-offers-microsoft-marketplace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-offers-openapi.json
- filename: tackle-contracts-openapi.json
  format: json
  label: Tackle Public Contracts API
  slug: tackle-public-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-contracts-openapi.json
- filename: tackle-prospect-openapi.json
  format: json
  label: Tackle Prospect API
  slug: tackle-prospect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-prospect-openapi.json
- filename: tackle-scim-openapi.json
  format: json
  label: Tackle SCIM API
  slug: tackle-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/openapi/tackle-scim-openapi.json
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Tackle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Tackle uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tackle
provider_slug: tackle
schemes:
- description: This auth-type is for `oauth2` client credentials flow. We will use the client_id and client_secret to call the token_url to get an access token; this is only used for `callbacks`'
  flows:
  - flow: clientCredentials
    tokenUrl: /oauth/token
  name: Oauth2AuthCallback
  source: openapi/tackle-api-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: tackle-scopes
source_filename: tackle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/tackle-api-openapi.json\nschemes:\n- name: Oauth2AuthCallback\n  source: openapi/tackle-api-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n  description: This auth-type is for `oauth2` client credentials flow. We will use the client_id\n    and client_secret to call the token_url to get an access token; this is only used for `callbacks`'\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tackle/refs/heads/main/scopes/tackle-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Cloud Marketplace
- Cloud GTM
- Go-To-Market
- Private Offers
- Co-Sell
- Metering
- SCIM
- AWS Marketplace
- Azure Marketplace
token_urls:
- /oauth/token
---
