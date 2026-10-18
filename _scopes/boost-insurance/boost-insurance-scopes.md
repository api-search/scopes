---
api_specs:
- filename: boost-insurance-authentication-api-openapi.yml
  format: yaml
  label: Boost Insurance Authentication API
  slug: boost-insurance-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-authentication-api-openapi.yml
- filename: boost-insurance-claims-api-openapi.yml
  format: yaml
  label: Boost Insurance Claims API
  slug: boost-insurance-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-claims-api-openapi.yml
- filename: boost-insurance-policies-api-openapi.yml
  format: yaml
  label: Boost Insurance Policies API
  slug: boost-insurance-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-policies-api-openapi.yml
- filename: boost-insurance-quotes-api-openapi.yml
  format: yaml
  label: Boost Insurance Quotes API
  slug: boost-insurance-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/openapi/boost-insurance-quotes-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Boost Insurance Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
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
  source: openapi/boost-insurance-authentication-api-openapi.yml
- description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication endpoint and presented as a Bearer token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.insurtech.dev/auth/oauth2/token
  name: boostOAuth
  source: openapi/boost-insurance-claims-api-openapi.yml
- description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication endpoint and presented as a Bearer token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.insurtech.dev/auth/oauth2/token
  name: boostOAuth
  source: openapi/boost-insurance-policies-api-openapi.yml
- description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication endpoint and presented as a Bearer token.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.insurtech.dev/auth/oauth2/token
  name: boostOAuth
  source: openapi/boost-insurance-quotes-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: boost-insurance-scopes
source_filename: boost-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/boost-insurance-authentication-api-openapi.yml, openapi/boost-insurance-claims-api-openapi.yml,\n  openapi/boost-insurance-policies-api-openapi.yml, openapi/boost-insurance-quotes-api-openapi.yml\nschemes:\n- name: boostOAuth\n  source: openapi/boost-insurance-authentication-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.insurtech.dev/auth/oauth2/token\n  description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication\n    endpoint and presented as a Bearer token.\n- name: boostOAuth\n  source: openapi/boost-insurance-claims-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.insurtech.dev/auth/oauth2/token\n  description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication\n    endpoint and presented as a Bearer token.\n- name: boostOAuth\n  source: openapi/boost-insurance-policies-api-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.insurtech.dev/auth/oauth2/token\n  description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication\n    endpoint and presented as a Bearer token.\n- name: boostOAuth\n  source: openapi/boost-insurance-quotes-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.insurtech.dev/auth/oauth2/token\n  description: OAuth 2.0 Client Credentials grant. Tokens are obtained from the Boost authentication\n    endpoint and presented as a Bearer token.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boost-insurance/refs/heads/main/scopes/boost-insurance-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Embedded Insurance
- Insurance As A Service
- Policy Administration
- Claims
token_bound: false
token_urls:
- https://api.insurtech.dev/auth/oauth2/token
---
