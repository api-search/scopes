---
api_specs:
- filename: weatherbys-bank-atm-api-openapi.yml
  format: yaml
  label: Weatherbys Bank ATM API
  slug: weatherbys-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/weatherbys-bank-atm-api-openapi.yml
- filename: weatherbys-bank-bca-api-openapi.yml
  format: yaml
  label: Weatherbys Bank BCA API
  slug: weatherbys-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/weatherbys-bank-bca-api-openapi.yml
- filename: weatherbys-bank-branch-api-openapi.yml
  format: yaml
  label: Weatherbys Bank Branch API
  slug: weatherbys-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/weatherbys-bank-branch-api-openapi.yml
- filename: weatherbys-bank-pca-api-openapi.yml
  format: yaml
  label: Weatherbys Bank PCA API
  slug: weatherbys-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/weatherbys-bank-pca-api-openapi.yml
authorization_urls: []
description: ''
docs: https://openbankinguk.github.io/read-write-api-site3/v3.1.11/profiles/read-write-data-api-profile.html
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Weatherbys Bank Scopes
name_suffix: OAuth Scopes
note: The OBIE Read/Write standard this ASPSP conforms to defines a fixed set of OAuth2 scopes for the AIS/PIS/CBPII surfaces. The Open Data APIs are public and have no scopes. Scopes are standardised by Open Banking Ltd, not bank-proprietary.
overview: 'Weatherbys Bank publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Weatherbys Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Weatherbys Bank
provider_slug: weatherbys-bank
schemes:
- applies_to:
  - AIS
  - PIS
  - CBPII
  flows:
  - authorizationCode
  - clientCredentials
  name: fapi-oauth2
scope_count: 4
scope_names:
- openid
- accounts
- payments
- fundsconfirmations
scopes:
- description: Required OpenID Connect scope for all Read/Write authorization flows.
  flows: []
  scope: openid
- description: Account and Transaction Information (AIS) — access to account, balance, transaction and related data.
  flows: []
  scope: accounts
- description: Payment Initiation (PIS) — create and manage domestic/international payment consents and payments.
  flows: []
  scope: payments
- description: Confirmation of Funds (CBPII) — confirm availability of funds against a consented account.
  flows: []
  scope: fundsconfirmations
slug: weatherbys-bank-scopes
source_filename: weatherbys-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://openbankinguk.github.io/read-write-api-site3/ (OBIE Read/Write API standard)\ndocs: https://openbankinguk.github.io/read-write-api-site3/v3.1.11/profiles/read-write-data-api-profile.html\nnote: >-\n  The OBIE Read/Write standard this ASPSP conforms to defines a fixed set of OAuth2\n  scopes for the AIS/PIS/CBPII surfaces. The Open Data APIs are public and have no\n  scopes. Scopes are standardised by Open Banking Ltd, not bank-proprietary.\nschemes:\n- name: fapi-oauth2\n  applies_to: [AIS, PIS, CBPII]\n  flows: [authorizationCode, clientCredentials]\nscopes:\n- scope: openid\n  description: Required OpenID Connect scope for all Read/Write authorization flows.\n  apis: [AIS, PIS, CBPII]\n- scope: accounts\n  description: Account and Transaction Information (AIS) — access to account, balance, transaction and related data.\n  apis: [AIS]\n- scope: payments\n  description: Payment Initiation (PIS) — create and manage domestic/international\
  \ payment consents and payments.\n  apis: [PIS]\n- scope: fundsconfirmations\n  description: Confirmation of Funds (CBPII) — confirm availability of funds against a consented account.\n  apis: [CBPII]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/scopes/weatherbys-bank-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Private Banking
token_urls: []
---
