---
api_specs:
- filename: mettle-open-data-api-openapi.json
  format: json
  label: Mettle Open Data Product API
  slug: mettle-open-data-product-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mettle/refs/heads/main/openapi/mettle-open-data-api-openapi.json
authorization_urls:
- https://secure1.natwest.com/as/authorization.oauth2
description: ''
docs: https://www.bankofapis.com/products/accounts/documentation/mettle
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Mettle Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mettle publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mettle API on a user''s behalf.


  Tokens are issued from https://secure1t.natwest.com/as/token.oauth2.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mettle
provider_slug: mettle
schemes:
- flows:
  - authorizationUrl: https://secure1.natwest.com/as/authorization.oauth2
    flow: authorizationCode
    tokenUrl: https://secure1t.natwest.com/as/token.oauth2
  - flow: clientCredentials
    tokenUrl: https://secure1t.natwest.com/as/token.oauth2
  name: OpenBankingOAuth2
  source: https://secure1.natwest.com/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- accounts
- payments
- fundsconfirmations
scopes:
- description: OpenID Connect - issue an id_token binding the consent (openbanking_intent_id).
  flows:
  - authorizationCode
  scope: openid
- description: Account & Transaction Information (AIS) - read accounts, balances, transactions, and related resources.
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: Payment Initiation (PIS) - create and submit domestic and other payment orders from a customer's account.
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: Confirmation of Funds (CBPII) - confirm whether funds are available on a customer's account.
  flows:
  - authorizationCode
  - clientCredentials
  scope: fundsconfirmations
slug: mettle-scopes
source_filename: mettle-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  https://secure1.natwest.com/.well-known/openid-configuration (scopes_supported)\n  filtered to Mettle's OBIE Read/Write products\ndocs: https://www.bankofapis.com/products/accounts/documentation/mettle\nnotes: >-\n  The NatWest Group OpenID Provider advertises a very large enterprise scope set;\n  the scopes below are the OBIE Read/Write standard scopes that apply to Mettle's\n  published AIS/PIS/CBPII products. A token request passes one or more of the\n  scopes the TPP has been granted, plus openid for the OIDC id_token.\nschemes:\n- name: OpenBankingOAuth2\n  source: https://secure1.natwest.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure1.natwest.com/as/authorization.oauth2\n    tokenUrl: https://secure1t.natwest.com/as/token.oauth2\n  - flow: clientCredentials\n    tokenUrl: https://secure1t.natwest.com/as/token.oauth2\nscopes:\n- scope: openid\n  description:\
  \ OpenID Connect - issue an id_token binding the consent (openbanking_intent_id).\n  flows: [authorizationCode]\n- scope: accounts\n  description: Account & Transaction Information (AIS) - read accounts, balances, transactions, and related resources.\n  flows: [authorizationCode, clientCredentials]\n  product: mettle-account-transaction-api\n- scope: payments\n  description: Payment Initiation (PIS) - create and submit domestic and other payment orders from a customer's account.\n  flows: [authorizationCode, clientCredentials]\n  product: mettle-payment-initiation-api\n- scope: fundsconfirmations\n  description: Confirmation of Funds (CBPII) - confirm whether funds are available on a customer's account.\n  flows: [authorizationCode, clientCredentials]\n  product: mettle-confirmation-of-funds-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mettle/refs/heads/main/scopes/mettle-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Financial Services
- Banking
- Business Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- Challenger Bank
- Fintech
token_urls:
- https://secure1t.natwest.com/as/token.oauth2
---
