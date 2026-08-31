---
api_specs:
- filename: virgin-money-uk-atm-api-openapi.yml
  format: yaml
  label: Virgin Money UK ATM API
  slug: virgin-money-uk-atm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/openapi/virgin-money-uk-atm-api-openapi.yml
- filename: virgin-money-uk-bca-api-openapi.yml
  format: yaml
  label: Virgin Money UK BCA API
  slug: virgin-money-uk-bca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/openapi/virgin-money-uk-bca-api-openapi.yml
- filename: virgin-money-uk-branch-api-openapi.yml
  format: yaml
  label: Virgin Money UK Branch API
  slug: virgin-money-uk-branch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/openapi/virgin-money-uk-branch-api-openapi.yml
- filename: virgin-money-uk-ccc-api-openapi.yml
  format: yaml
  label: Virgin Money UK CCC API
  slug: virgin-money-uk-ccc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/openapi/virgin-money-uk-ccc-api-openapi.yml
- filename: virgin-money-uk-pca-api-openapi.yml
  format: yaml
  label: Virgin Money UK PCA API
  slug: virgin-money-uk-pca-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/openapi/virgin-money-uk-pca-api-openapi.yml
- filename: virgin-money-uk-sme-api-openapi.yml
  format: yaml
  label: Virgin Money UK SME API
  slug: virgin-money-uk-sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/openapi/virgin-money-uk-sme-api-openapi.yml
authorization_urls:
- https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/authorize
description: ''
docs: https://developer.virginmoney.com/merged/oidc/
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Virgin Money Uk Scopes
name_suffix: OAuth Scopes
note: Scopes taken verbatim from the live production OpenID Connect discovery document (scopes_supported). These are the standard UK Open Banking / OBIE Read-Write scopes governing AIS, PIS, and CBPII access.
overview: 'Virgin Money UK publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Virgin Money UK API on a user''s behalf.


  Tokens are issued from https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Virgin Money UK
provider_slug: virgin-money-uk
schemes:
- flows:
  - authorizationUrl: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token
  name: OAuth2
  source: well-known/virgin-money-uk-openid-configuration.json
scope_count: 4
scope_names:
- openid
- accounts
- payments
- fundsconfirmations
scopes:
- description: OpenID Connect authentication; required to obtain an ID token identifying the consent.
  flows:
  - authorizationCode
  scope: openid
- description: Account and Transaction Information (AIS) — read accounts, balances, transactions, beneficiaries, standing orders, direct debits, statements.
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: Payment Initiation (PIS) — initiate domestic/international immediate, scheduled, and file payments.
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: Confirmation of Funds (CBPII) — confirm whether sufficient funds are available to make a card-based payment.
  flows:
  - authorizationCode
  - clientCredentials
  scope: fundsconfirmations
slug: virgin-money-uk-scopes
source_filename: virgin-money-uk-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: well-known/virgin-money-uk-openid-configuration.json\ndocs: https://developer.virginmoney.com/merged/oidc/\nnote: >-\n  Scopes taken verbatim from the live production OpenID Connect discovery document\n  (scopes_supported). These are the standard UK Open Banking / OBIE Read-Write\n  scopes governing AIS, PIS, and CBPII access.\nschemes:\n- name: OAuth2\n  source: well-known/virgin-money-uk-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/authorize\n    tokenUrl: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; required to obtain an ID token identifying\
  \ the consent.\n  flows: [authorizationCode]\n  sources: [well-known/virgin-money-uk-openid-configuration.json]\n- scope: accounts\n  description: >-\n    Account and Transaction Information (AIS) — read accounts, balances,\n    transactions, beneficiaries, standing orders, direct debits, statements.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/virgin-money-uk-openid-configuration.json]\n- scope: payments\n  description: >-\n    Payment Initiation (PIS) — initiate domestic/international immediate,\n    scheduled, and file payments.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/virgin-money-uk-openid-configuration.json]\n- scope: fundsconfirmations\n  description: >-\n    Confirmation of Funds (CBPII) — confirm whether sufficient funds are\n    available to make a card-based payment.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/virgin-money-uk-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-money-uk/refs/heads/main/scopes/virgin-money-uk-scopes.yml
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
- Confirmation of Funds
- FAPI
token_urls:
- https://secureapi.prod.ob.virginmoney.com/vmpsd2-psd2prod/psd2-production/oidcapi/oauth2/token
---
