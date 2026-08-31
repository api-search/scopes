---
api_specs:
- filename: allica-bank-account-access-api-openapi.yml
  format: yaml
  label: Allica Bank Account Access API
  slug: allica-bank-account-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-account-access-api-openapi.yml
- filename: allica-bank-accounts-api-openapi.yml
  format: yaml
  label: Allica Bank Accounts API
  slug: allica-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-accounts-api-openapi.yml
- filename: allica-bank-balances-api-openapi.yml
  format: yaml
  label: Allica Bank Balances API
  slug: allica-bank-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-balances-api-openapi.yml
- filename: allica-bank-beneficiaries-api-openapi.yml
  format: yaml
  label: Allica Bank Beneficiaries API
  slug: allica-bank-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-beneficiaries-api-openapi.yml
- filename: allica-bank-direct-debits-api-openapi.yml
  format: yaml
  label: Allica Bank Direct Debits API
  slug: allica-bank-direct-debits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-direct-debits-api-openapi.yml
- filename: allica-bank-domestic-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Payments API
  slug: allica-bank-domestic-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-payments-api-openapi.yml
- filename: allica-bank-domestic-scheduled-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Scheduled Payments API
  slug: allica-bank-domestic-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-scheduled-payments-api-openapi.yml
- filename: allica-bank-domestic-standing-orders-api-openapi.yml
  format: yaml
  label: Allica Bank Domestic Standing Orders API
  slug: allica-bank-domestic-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-domestic-standing-orders-api-openapi.yml
- filename: allica-bank-file-payments-api-openapi.yml
  format: yaml
  label: Allica Bank File Payments API
  slug: allica-bank-file-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-file-payments-api-openapi.yml
- filename: allica-bank-offers-api-openapi.yml
  format: yaml
  label: Allica Bank Offers API
  slug: allica-bank-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-offers-api-openapi.yml
- filename: allica-bank-parties-api-openapi.yml
  format: yaml
  label: Allica Bank Parties API
  slug: allica-bank-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-parties-api-openapi.yml
- filename: allica-bank-payment-details-api-openapi.yml
  format: yaml
  label: Allica Bank Payment Details API
  slug: allica-bank-payment-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-payment-details-api-openapi.yml
- filename: allica-bank-products-api-openapi.yml
  format: yaml
  label: Allica Bank Products API
  slug: allica-bank-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-products-api-openapi.yml
- filename: allica-bank-scheduled-payments-api-openapi.yml
  format: yaml
  label: Allica Bank Scheduled Payments API
  slug: allica-bank-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-scheduled-payments-api-openapi.yml
- filename: allica-bank-standing-orders-api-openapi.yml
  format: yaml
  label: Allica Bank Standing Orders API
  slug: allica-bank-standing-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-standing-orders-api-openapi.yml
- filename: allica-bank-transactions-api-openapi.yml
  format: yaml
  label: Allica Bank Transactions API
  slug: allica-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/openapi/allica-bank-transactions-api-openapi.yml
authorization_urls:
- https://secure.allica.bank/open-banking
description: ''
docs: https://auth1.api.ob.allica.bank/.well-known/openid-configuration
flows:
- clientCredentials
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Allica Bank Scopes
name_suffix: OAuth Scopes
note: The OpenAPI specs declare OBIE oauth2 security schemes (TPP client-credentials + PSU authorization-code) with placeholder authserver.example URLs. Real flow endpoints and the full scope set were confirmed live from Allica's production FAPI OIDC discovery document (scopes_supported), captured verbatim in well-known/allica-bank-openid-configuration.json. These are OBIE Read/Write Open Banking scopes; access is FAPI/mTLS-gated and requires OBIE Directory onboarding.
overview: 'Allica Bank publishes 17 OAuth 2.0 scopes via the clientCredentials and authorizationCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Allica Bank API on a user''s behalf.


  Tokens are issued from https://as1.api.ob.allica.bank/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Allica Bank
provider_slug: allica-bank
schemes:
- description: TPP client-credentials authorisation flow with the ASPSP (grant for consent creation / non-PSU resources).
  flows:
  - flow: clientCredentials
    tokenUrl: https://as1.api.ob.allica.bank/token
  name: TPPOAuth2Security
  source: openapi + OIDC discovery
  type: oauth2
- description: OAuth authorization-code flow requiring PSU strong customer authentication (SCA) to access PSU-owned ASPSP resources.
  flows:
  - authorizationUrl: https://secure.allica.bank/open-banking
    flow: authorizationCode
    tokenUrl: https://as1.api.ob.allica.bank/token
  name: PSUOAuth2Security
  source: openapi + OIDC discovery
  type: oauth2
scope_count: 17
scope_names:
- openid
- accounts
- payments
- fundsconfirmations
- consents
- resources
- credit-cards-accounts
- customers
- loans
- financings
- invoice-financings
- unarranged-accounts-overdraft
- consumption
- lg
- recurring-payments
- bank-fixed-incomes
- recurring-consent
scopes:
- description: OpenID Connect authentication; returns an id_token identifying the authenticated PSU consent.
  flows:
  - authorizationCode
  scope: openid
- description: Read access to Account and Transaction Information (AIS) resources for Allica Business Rewards accounts.
  flows:
  - authorizationCode
  - clientCredentials
  scope: accounts
- description: Initiate and read domestic payments, scheduled payments, and standing orders (PIS).
  flows:
  - authorizationCode
  - clientCredentials
  scope: payments
- description: Confirm availability of funds on an account (Confirmation of Funds / CBPII).
  flows:
  - authorizationCode
  - clientCredentials
  scope: fundsconfirmations
- description: Manage the consent lifecycle (account-access, payment, and funds-confirmation consents).
  flows:
  - clientCredentials
  scope: consents
- description: General OBIE resource-access scope covering account resource discovery.
  flows:
  - clientCredentials
  scope: resources
- description: Access to credit-card account information resources (OBIE / Open Finance scope).
  flows:
  - authorizationCode
  scope: credit-cards-accounts
- description: Access to customer/party identity resources.
  flows:
  - authorizationCode
  scope: customers
- description: Access to loan account resources (Open Finance scope).
  flows:
  - authorizationCode
  scope: loans
- description: Access to financing product resources (asset/commercial finance).
  flows:
  - authorizationCode
  scope: financings
- description: Access to invoice-financing product resources.
  flows:
  - authorizationCode
  scope: invoice-financings
- description: Access to unarranged overdraft resources on accounts (Open Finance scope).
  flows:
  - authorizationCode
  scope: unarranged-accounts-overdraft
- description: Access to consumption/usage resources (Open Finance scope).
  flows:
  - authorizationCode
  scope: consumption
- description: Bank guarantees (letters of guarantee) resource scope (Open Finance).
  flows:
  - authorizationCode
  scope: lg
- description: Recurring-payments resource scope.
  flows:
  - authorizationCode
  - clientCredentials
  scope: recurring-payments
- description: Access to fixed-income investment product resources (Open Finance scope).
  flows:
  - authorizationCode
  scope: bank-fixed-incomes
- description: Manage recurring/long-lived consent resources.
  flows:
  - clientCredentials
  scope: recurring-consent
slug: allica-bank-scopes
source_filename: allica-bank-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: openapi/allica-bank-account-information-openapi.yaml, openapi/allica-bank-payment-initiation-openapi.yaml\ndocs: https://auth1.api.ob.allica.bank/.well-known/openid-configuration\nnote: |\n  The OpenAPI specs declare OBIE oauth2 security schemes (TPP client-credentials +\n  PSU authorization-code) with placeholder authserver.example URLs. Real flow\n  endpoints and the full scope set were confirmed live from Allica's production\n  FAPI OIDC discovery document (scopes_supported), captured verbatim in\n  well-known/allica-bank-openid-configuration.json. These are OBIE Read/Write\n  Open Banking scopes; access is FAPI/mTLS-gated and requires OBIE Directory\n  onboarding.\nschemes:\n- name: TPPOAuth2Security\n  type: oauth2\n  source: openapi + OIDC discovery\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://as1.api.ob.allica.bank/token\n  description: TPP client-credentials authorisation flow with the ASPSP (grant\
  \ for consent creation / non-PSU resources).\n- name: PSUOAuth2Security\n  type: oauth2\n  source: openapi + OIDC discovery\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.allica.bank/open-banking\n    tokenUrl: https://as1.api.ob.allica.bank/token\n  description: OAuth authorization-code flow requiring PSU strong customer authentication (SCA) to access PSU-owned ASPSP resources.\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an id_token identifying the authenticated PSU consent.\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n- scope: accounts\n  description: Read access to Account and Transaction Information (AIS) resources for Allica Business Rewards accounts.\n  flows: [authorizationCode, clientCredentials]\n  sources: [openapi/allica-bank-account-information-openapi.yaml, OIDC discovery]\n- scope: payments\n  description: Initiate and read domestic payments, scheduled payments, and standing orders (PIS).\n\
  \  flows: [authorizationCode, clientCredentials]\n  sources: [openapi/allica-bank-payment-initiation-openapi.yaml, OIDC discovery]\n- scope: fundsconfirmations\n  description: Confirm availability of funds on an account (Confirmation of Funds / CBPII).\n  flows: [authorizationCode, clientCredentials]\n  sources: [OIDC discovery]\n- scope: consents\n  description: Manage the consent lifecycle (account-access, payment, and funds-confirmation consents).\n  flows: [clientCredentials]\n  sources: [OIDC discovery]\n- scope: resources\n  description: General OBIE resource-access scope covering account resource discovery.\n  flows: [clientCredentials]\n  sources: [OIDC discovery]\n- scope: credit-cards-accounts\n  description: Access to credit-card account information resources (OBIE / Open Finance scope).\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n- scope: customers\n  description: Access to customer/party identity resources.\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n\
  - scope: loans\n  description: Access to loan account resources (Open Finance scope).\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n- scope: financings\n  description: Access to financing product resources (asset/commercial finance).\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n- scope: invoice-financings\n  description: Access to invoice-financing product resources.\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n- scope: unarranged-accounts-overdraft\n  description: Access to unarranged overdraft resources on accounts (Open Finance scope).\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n- scope: consumption\n  description: Access to consumption/usage resources (Open Finance scope).\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n- scope: lg\n  description: Bank guarantees (letters of guarantee) resource scope (Open Finance).\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n- scope: recurring-payments\n  description:\
  \ Recurring-payments resource scope.\n  flows: [authorizationCode, clientCredentials]\n  sources: [OIDC discovery]\n- scope: bank-fixed-incomes\n  description: Access to fixed-income investment product resources (Open Finance scope).\n  flows: [authorizationCode]\n  sources: [OIDC discovery]\n- scope: recurring-consent\n  description: Manage recurring/long-lived consent resources.\n  flows: [clientCredentials]\n  sources: [OIDC discovery]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/allica-bank/refs/heads/main/scopes/allica-bank-scopes.yml
summary_line: 17 scopes · clientCredentials/authorizationCode
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- OBIE
- FAPI
- United Kingdom
- Payments
- Account Information
- SME
- Business Banking
- Fintech
token_urls:
- https://as1.api.ob.allica.bank/token
---
