---
api_specs:
- filename: landmark-information-order-experience-api-openapi.yml
  format: yaml
  label: Landmark Order Experience API
  slug: landmark-order-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-order-experience-api-openapi.yml
- filename: landmark-information-conveyancing-experience-api-openapi.yml
  format: yaml
  label: Landmark Conveyancing Experience API
  slug: landmark-conveyancing-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-conveyancing-experience-api-openapi.yml
- filename: landmark-information-intelliworks-api-openapi.yml
  format: yaml
  label: Landmark Intelliworks APIs
  slug: landmark-intelliworks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-intelliworks-api-openapi.yml
- filename: landmark-information-document-vault-api-openapi.yml
  format: yaml
  label: Landmark Document Vault API
  slug: landmark-document-vault-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-document-vault-api-openapi.yml
- filename: landmark-information-milestone-notification-service-api-openapi.yml
  format: yaml
  label: Landmark Milestone Notification Service API
  slug: landmark-milestone-notification-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/openapi/landmark-information-milestone-notification-service-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Landmark Information Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Landmark Information Group uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://lmkmaster.eu.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Landmark Information Group
provider_slug: landmark-information
schemes:
- description: 'OAuth 2.0 client credentials. Request an access token from the token endpoint for your

    environment, then send it as a bearer token on every request. See **Authentication** for details.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://lmkmaster.eu.auth0.com/oauth/token
  name: BearerAuth
  source: openapi/landmark-information-conveyancing-experience-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: landmark-information-scopes
source_filename: landmark-information-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: derived\nsource: openapi/landmark-information-conveyancing-experience-api-openapi.yml\nschemes:\n- name: BearerAuth\n  source: openapi/landmark-information-conveyancing-experience-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://lmkmaster.eu.auth0.com/oauth/token\n  description: |-\n    OAuth 2.0 client credentials. Request an access token from the token endpoint for your\n    environment, then send it as a bearer token on every request. See **Authentication** for details.\nscopes: []\nnotes: >-\n  Landmark declares an OAuth 2.0 client-credentials scheme in the Conveyancing Experience API but\n  publishes an empty scopes map, and no scope or permission reference page exists on the public\n  documentation portal. Authorisation is carried by entitlements attached to the onboarded account\n  and audience rather than by OAuth scopes - a 403 with code 40300/40301 (\"Invalid Entitlement\" /\n  \"No Entitlement\") is how\
  \ the platform signals an unauthorised operation. See\n  authentication/landmark-information-authentication.yml for the working model.\n\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landmark-information/refs/heads/main/scopes/landmark-information-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Real-Estate
- United Kingdom
- PropTech
- Property Data
- Conveyancing
- Land Registry
- Geospatial
- Valuation
- Anti-Money Laundering
- Planning Data
- Mortgage
token_urls:
- https://lmkmaster.eu.auth0.com/oauth/token
---
