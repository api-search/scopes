---
api_specs:
- filename: metro-bank-atm-api-openapi.yml
  format: yaml
  label: Metro Bank ATM API
  slug: metro-bank-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-atm-api-openapi.yml
- filename: metro-bank-bca-api-openapi.yml
  format: yaml
  label: Metro Bank BCA API
  slug: metro-bank-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-bca-api-openapi.yml
- filename: metro-bank-branch-api-openapi.yml
  format: yaml
  label: Metro Bank Branch API
  slug: metro-bank-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-branch-api-openapi.yml
- filename: metro-bank-ccc-api-openapi.yml
  format: yaml
  label: Metro Bank CCC API
  slug: metro-bank-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-ccc-api-openapi.yml
- filename: metro-bank-pca-api-openapi.yml
  format: yaml
  label: Metro Bank PCA API
  slug: metro-bank-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-pca-api-openapi.yml
- filename: metro-bank-sme-api-openapi.yml
  format: yaml
  label: Metro Bank SME API
  slug: metro-bank-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/openapi/metro-bank-sme-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.metrobankonline.co.uk/Overview
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Metro Bank Scopes
name_suffix: OAuth Scopes
note: These are the standardised OBIE UK Open Banking Read/Write scopes that Metro Bank's FAPI-secured AIS/PIS/CBPII APIs use. Live introspection of Metro's own authorization server is mTLS/edge-gated and could not be performed anonymously; scopes are captured from the OBIE standard the bank conforms to.
overview: 'Metro Bank publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Metro Bank API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Metro Bank
provider_slug: metro-bank
schemes:
- flows:
  - flow: authorizationCode
    note: FAPI OIDC hybrid; customer-present with PSD2 SCA
  - flow: clientCredentials
    note: consent-resource creation
  name: OBIE-FAPI-OAuth2
  source: OBIE Read/Write API Security Profile
scope_count: 4
scope_names:
- openid
- accounts
- payments
- fundsconfirmations
scopes:
- description: OpenID Connect scope; required to obtain an id_token and run the FAPI OIDC hybrid authorisation flow.
  flows:
  - authorizationCode
  scope: openid
- description: Account and Transaction Information (AIS) - consented read access to accounts, balances, transactions, beneficiaries, standing orders, direct debits, statements, and party data.
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: Payment Initiation (PIS) - create and submit domestic, scheduled, standing-order and file payment-consent and payment resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: Confirmation of Funds (CBPII) - confirm whether sufficient funds are available on a customer account for a card-based payment instrument.
  flows:
  - authorizationCode
  - clientCredentials
  scope: fundsconfirmations
slug: metro-bank-scopes
source_filename: metro-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  OBIE Read/Write API Specification (github.com/OpenBankingUK/read-write-api-specs)\n  - Metro Bank's AIS/PIS/CBPII APIs conform to this standard. The Open Data API\n  is unauthenticated and declares no scopes.\ndocs: https://developer.metrobankonline.co.uk/Overview\nschemes:\n  - name: OBIE-FAPI-OAuth2\n    source: OBIE Read/Write API Security Profile\n    flows:\n      - flow: authorizationCode\n        note: FAPI OIDC hybrid; customer-present with PSD2 SCA\n      - flow: clientCredentials\n        note: consent-resource creation\nscopes:\n  - scope: openid\n    description: >-\n      OpenID Connect scope; required to obtain an id_token and run the\n      FAPI OIDC hybrid authorisation flow.\n    flows: [authorizationCode]\n    sources: [OBIE Read/Write API Security Profile]\n  - scope: accounts\n    description: >-\n      Account and Transaction Information (AIS) - consented read access to\n      accounts, balances,\
  \ transactions, beneficiaries, standing orders,\n      direct debits, statements, and party data.\n    flows: [authorizationCode, clientCredentials]\n    api: metro-bank:metro-bank-account-information-api\n    sources: [OBIE Read/Write API Security Profile]\n  - scope: payments\n    description: >-\n      Payment Initiation (PIS) - create and submit domestic, scheduled,\n      standing-order and file payment-consent and payment resources.\n    flows: [authorizationCode, clientCredentials]\n    api: metro-bank:metro-bank-payment-initiation-api\n    sources: [OBIE Read/Write API Security Profile]\n  - scope: fundsconfirmations\n    description: >-\n      Confirmation of Funds (CBPII) - confirm whether sufficient funds are\n      available on a customer account for a card-based payment instrument.\n    flows: [authorizationCode, clientCredentials]\n    api: metro-bank:metro-bank-confirmation-of-funds-api\n    sources: [OBIE Read/Write API Security Profile]\nnote: >-\n  These are the standardised\
  \ OBIE UK Open Banking Read/Write scopes that Metro\n  Bank's FAPI-secured AIS/PIS/CBPII APIs use. Live introspection of Metro's own\n  authorization server is mTLS/edge-gated and could not be performed anonymously;\n  scopes are captured from the OBIE standard the bank conforms to.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metro-bank/refs/heads/main/scopes/metro-bank-scopes.yml
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
- FAPI
- Fintech
token_urls: []
---
