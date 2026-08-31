---
api_specs:
- filename: algbra-account-access-api-openapi.yml
  format: yaml
  label: Algbra Account Access API
  slug: algbra-account-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/openapi/algbra-account-access-api-openapi.yml
- filename: algbra-accounts-api-openapi.yml
  format: yaml
  label: Algbra Accounts API
  slug: algbra-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/openapi/algbra-accounts-api-openapi.yml
- filename: algbra-balances-api-openapi.yml
  format: yaml
  label: Algbra Balances API
  slug: algbra-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/openapi/algbra-balances-api-openapi.yml
- filename: algbra-beneficiaries-api-openapi.yml
  format: yaml
  label: Algbra Beneficiaries API
  slug: algbra-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/openapi/algbra-beneficiaries-api-openapi.yml
- filename: algbra-transactions-api-openapi.yml
  format: yaml
  label: Algbra Transactions API
  slug: algbra-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/openapi/algbra-transactions-api-openapi.yml
authorization_urls:
- https://secure.tell.systems/algbra/auth/oidc/authorize
description: ''
docs: https://developer.algbralabs.com/open-banking-uk/introduction
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Algbra Scopes
name_suffix: OAuth Scopes
note: OAuth2 schemes/scope 'accounts' derived from the harvested AIS spec; the additional OBIE scopes (openid, payments, fundsconfirmations) are documented in Algbra's Open Banking security model and the OBIE Read/Write Standard for the PIS/CBPII surfaces, which are not separately specified.
overview: 'Algbra publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Algbra API on a user''s behalf.


  Tokens are issued from https://secure.tell.systems/algbra/auth/oidc/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Algbra
provider_slug: algbra
schemes:
- description: PSU authorization-code flow requiring SCA with the ASPSP.
  flows:
  - authorizationUrl: https://secure.tell.systems/algbra/auth/oidc/authorize
    flow: authorizationCode
    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token
  name: PSUOAuth2Security
  source: openapi/algbra-account-transaction-api-openapi.yml
- description: TPP client-credentials authorisation flow with the ASPSP.
  flows:
  - flow: clientCredentials
    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token
  name: TPPOAuth2Security
  source: openapi/algbra-account-transaction-api-openapi.yml
scope_count: 4
scope_names:
- accounts
- openid
- payments
- fundsconfirmations
scopes:
- description: Read access to accounts, balances, beneficiaries and transactions (AIS).
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: OpenID Connect authentication (id_token) as part of the FAPI flow.
  flows:
  - authorizationCode
  scope: openid
- description: Initiate payments on the customer's behalf (PIS) - documented, not separately specified.
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: Confirm availability of funds (CBPII) - documented, not separately specified.
  flows:
  - clientCredentials
  scope: fundsconfirmations
slug: algbra-scopes
source_filename: algbra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/algbra-account-transaction-api-openapi.yml\ndocs: https://developer.algbralabs.com/open-banking-uk/introduction\nnote: >-\n  OAuth2 schemes/scope 'accounts' derived from the harvested AIS spec; the additional\n  OBIE scopes (openid, payments, fundsconfirmations) are documented in Algbra's Open\n  Banking security model and the OBIE Read/Write Standard for the PIS/CBPII surfaces,\n  which are not separately specified.\nschemes:\n- name: PSUOAuth2Security\n  source: openapi/algbra-account-transaction-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.tell.systems/algbra/auth/oidc/authorize\n    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token\n  description: PSU authorization-code flow requiring SCA with the ASPSP.\n- name: TPPOAuth2Security\n  source: openapi/algbra-account-transaction-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://secure.tell.systems/algbra/auth/oidc/token\n\
  \  description: TPP client-credentials authorisation flow with the ASPSP.\nscopes:\n- scope: accounts\n  description: Read access to accounts, balances, beneficiaries and transactions (AIS).\n  flows: [authorizationCode, clientCredentials]\n  sources: [openapi/algbra-account-transaction-api-openapi.yml]\n- scope: openid\n  description: OpenID Connect authentication (id_token) as part of the FAPI flow.\n  flows: [authorizationCode]\n  sources: [docs]\n- scope: payments\n  description: Initiate payments on the customer's behalf (PIS) - documented, not separately specified.\n  flows: [authorizationCode, clientCredentials]\n  sources: [docs]\n- scope: fundsconfirmations\n  description: Confirm availability of funds (CBPII) - documented, not separately specified.\n  flows: [clientCredentials]\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/algbra/refs/heads/main/scopes/algbra-scopes.yml
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
- Fintech
- Ethical Finance
- Banking as a Service
token_urls:
- https://secure.tell.systems/algbra/auth/oidc/token
---
