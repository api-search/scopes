---
api_specs:
- filename: halifax-atm-api-openapi.yml
  format: yaml
  label: Halifax ATM API
  slug: halifax-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/halifax-atm-api-openapi.yml
- filename: halifax-bca-api-openapi.yml
  format: yaml
  label: Halifax BCA API
  slug: halifax-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/halifax-bca-api-openapi.yml
- filename: halifax-branch-api-openapi.yml
  format: yaml
  label: Halifax Branch API
  slug: halifax-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/halifax-branch-api-openapi.yml
- filename: halifax-ccc-api-openapi.yml
  format: yaml
  label: Halifax CCC API
  slug: halifax-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/halifax-ccc-api-openapi.yml
- filename: halifax-pca-api-openapi.yml
  format: yaml
  label: Halifax PCA API
  slug: halifax-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/halifax-pca-api-openapi.yml
- filename: halifax-sme-api-openapi.yml
  format: yaml
  label: Halifax SME API
  slug: halifax-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/openapi/halifax-sme-api-openapi.yml
authorization_urls: []
description: ''
docs: https://openbankinguk.github.io/read-write-api-site3/v3.1.11/profiles/read-write-data-api-profile.html
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Halifax Scopes
name_suffix: OAuth Scopes
note: OBIE Read/Write standard scopes for the FAPI-secured AIS/PIS/CBPII APIs. Not derivable from the captured Open Data swagger (which is public and declares no oauth2 securityScheme); sourced from the OBIE Read/Write standard and the Lloyds Banking Group Developer Portal. The Open Data APIs require no scopes.
overview: 'Halifax publishes 4 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Halifax API on a user''s behalf.


  Tokens are issued from https://authorise.<gated>/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Halifax
provider_slug: halifax
schemes:
- flows:
  - flow: clientCredentials
    note: Token URL is provisioned per-TPP via the Lloyds Developer Portal / OB Directory; not publicly published.
    tokenUrl: https://authorise.<gated>/token
  - flow: authorizationCode
    note: Authorization + token endpoints discovered per-brand via OIDC; onboarding-gated.
  name: OAuth2
scope_count: 4
scope_names:
- openid
- accounts
- payments
- fundsconfirmation
scopes:
- description: OpenID Connect authentication of the payment service user (PSU).
  flows:
  - authorizationCode
  scope: openid
- description: Account and Transaction Information (AIS). Read account, balance, transaction, beneficiary, standing-order, direct-debit, product, offer, party, scheduled-payment and statement data under an account-access-consent.
  flows:
  - clientCredentials
  - authorizationCode
  scope: accounts
- description: Payment Initiation (PIS). Set up and submit domestic, international, scheduled, standing-order and (where supported) variable-recurring payments under a payment consent. Refresh tokens supported for VRP.
  flows:
  - clientCredentials
  - authorizationCode
  scope: payments
- description: Confirmation of Funds (CBPII). Confirm whether funds are available for a specified amount on a PSU account under a funds-confirmation-consent.
  flows:
  - clientCredentials
  - authorizationCode
  scope: fundsconfirmation
slug: halifax-scopes
source_filename: halifax-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://developer.lloydsbanking.com/prod01/lbg/read-write\ndocs: https://openbankinguk.github.io/read-write-api-site3/v3.1.11/profiles/read-write-data-api-profile.html\nnote: >-\n  OBIE Read/Write standard scopes for the FAPI-secured AIS/PIS/CBPII APIs.\n  Not derivable from the captured Open Data swagger (which is public and\n  declares no oauth2 securityScheme); sourced from the OBIE Read/Write standard\n  and the Lloyds Banking Group Developer Portal. The Open Data APIs require no\n  scopes.\nschemes:\n  - name: OAuth2\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://authorise.<gated>/token\n        note: Token URL is provisioned per-TPP via the Lloyds Developer Portal / OB Directory; not publicly published.\n      - flow: authorizationCode\n        note: Authorization + token endpoints discovered per-brand via OIDC; onboarding-gated.\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication\
  \ of the payment service user (PSU).\n    flows: [authorizationCode]\n  - scope: accounts\n    description: >-\n      Account and Transaction Information (AIS). Read account, balance,\n      transaction, beneficiary, standing-order, direct-debit, product, offer,\n      party, scheduled-payment and statement data under an account-access-consent.\n    flows: [clientCredentials, authorizationCode]\n    apis: [halifax-account-transaction-information-api]\n  - scope: payments\n    description: >-\n      Payment Initiation (PIS). Set up and submit domestic, international,\n      scheduled, standing-order and (where supported) variable-recurring\n      payments under a payment consent. Refresh tokens supported for VRP.\n    flows: [clientCredentials, authorizationCode]\n    apis: [halifax-payment-initiation-api]\n  - scope: fundsconfirmation\n    description: >-\n      Confirmation of Funds (CBPII). Confirm whether funds are available for a\n      specified amount on a PSU account under a funds-confirmation-consent.\n\
  \    flows: [clientCredentials, authorizationCode]\n    apis: [halifax-confirmation-of-funds-api]\nrefresh_tokens_supported: [accounts, payments, fundsconfirmation]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/halifax/refs/heads/main/scopes/halifax-scopes.yml
summary_line: 4 scopes · clientCredentials/authorizationCode
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
- Open Data
token_urls:
- https://authorise.<gated>/token
---
