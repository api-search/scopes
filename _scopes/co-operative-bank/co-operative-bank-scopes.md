---
api_specs:
- filename: obie-open-data-api-standard-swagger.json
  format: json
  label: The Co-operative Bank Open Data API (OBIE standard)
  slug: open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/openapi/obie-open-data-api-standard-swagger.json
authorization_urls:
- https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/auth
description: ''
docs: https://www.developer.co-operativebank.co.uk/apis/general-specifications/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Co Operative Bank Scopes
name_suffix: OAuth Scopes
note: The bank's authorization server advertises only openid/offline_access/offline in its OIDC discovery document; the accounts/payments/fundsconfirmation scopes are the OBIE Read/Write 3.1 standard scopes that gate the corresponding consent + resource endpoints and are documented as OBIE standard, not verified in the discovery document.
overview: 'The Co-operative Bank publishes 6 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the The Co-operative Bank API on a user''s behalf.


  Tokens are issued from https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: The Co-operative Bank
provider_slug: co-operative-bank
schemes:
- flows:
  - authorizationUrl: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/token
  name: OpenBankingOAuth2
scope_count: 6
scope_names:
- openid
- offline_access
- offline
- accounts
- payments
- fundsconfirmation
scopes:
- description: OpenID Connect authentication; required to obtain an id_token for the PSU.
  flows:
  - authorizationCode
  scope: openid
- description: Request a refresh token so the TPP can obtain new access tokens without re-authenticating the PSU (within the consent window).
  flows:
  - authorizationCode
  scope: offline_access
- description: Offline access variant advertised by the authorization server.
  flows:
  - authorizationCode
  scope: offline
- description: OBIE Read/Write account-information (AIS) scope requested at the token endpoint alongside a signed account-access-consent, gating accounts, balances, transactions, direct debits, standing orders and scheduled payments. (OBIE Read/Write standard scope; not enumerated in the OIDC discovery document but required by the AISP flow.)
  flows:
  - authorizationCode
  scope: accounts
- description: OBIE Read/Write payment-initiation (PIS) scope requested alongside a signed payment-order consent for domestic payments, scheduled payments and standing orders. (OBIE Read/Write standard scope.)
  flows:
  - authorizationCode
  scope: payments
- description: OBIE Read/Write confirmation-of-funds (CBPII) scope requested alongside a funds-confirmation consent. (OBIE Read/Write standard scope.)
  flows:
  - authorizationCode
  scope: fundsconfirmation
slug: co-operative-bank-scopes
source_filename: co-operative-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://openbanking-retail.apis.co-operativebank.co.uk/apis/oauth/v1/.well-known/openid-configuration\ndocs: https://www.developer.co-operativebank.co.uk/apis/general-specifications/\nschemes:\n- name: OpenBankingOAuth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/auth\n    tokenUrl: https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; required to obtain an id_token for the PSU.\n  flows: [authorizationCode]\n  source: openid-configuration scopes_supported\n- scope: offline_access\n  description: Request a refresh token so the TPP can obtain new access tokens without re-authenticating the PSU (within the consent window).\n  flows: [authorizationCode]\n  source: openid-configuration scopes_supported\n- scope: offline\n  description: Offline access\
  \ variant advertised by the authorization server.\n  flows: [authorizationCode]\n  source: openid-configuration scopes_supported\n- scope: accounts\n  description: >-\n    OBIE Read/Write account-information (AIS) scope requested at the token\n    endpoint alongside a signed account-access-consent, gating accounts,\n    balances, transactions, direct debits, standing orders and scheduled\n    payments. (OBIE Read/Write standard scope; not enumerated in the OIDC\n    discovery document but required by the AISP flow.)\n  flows: [authorizationCode]\n  source: OBIE Read/Write 3.1 standard\n- scope: payments\n  description: >-\n    OBIE Read/Write payment-initiation (PIS) scope requested alongside a signed\n    payment-order consent for domestic payments, scheduled payments and standing\n    orders. (OBIE Read/Write standard scope.)\n  flows: [authorizationCode]\n  source: OBIE Read/Write 3.1 standard\n- scope: fundsconfirmation\n  description: >-\n    OBIE Read/Write confirmation-of-funds\
  \ (CBPII) scope requested alongside a\n    funds-confirmation consent. (OBIE Read/Write standard scope.)\n  flows: [authorizationCode]\n  source: OBIE Read/Write 3.1 standard\nnote: >-\n  The bank's authorization server advertises only openid/offline_access/offline\n  in its OIDC discovery document; the accounts/payments/fundsconfirmation scopes\n  are the OBIE Read/Write 3.1 standard scopes that gate the corresponding\n  consent + resource endpoints and are documented as OBIE standard, not verified\n  in the discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/co-operative-bank/refs/heads/main/scopes/co-operative-bank-scopes.yml
summary_line: 6 scopes · authorizationCode
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Fintech
token_urls:
- https://bank-retail.apis.co-operativebank.co.uk/apis/oauth/v1/oauth2/token
---
