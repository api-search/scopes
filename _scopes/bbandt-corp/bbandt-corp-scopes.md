---
api_specs:
- filename: bbandt-corp-commercial-accounts-openapi.yml
  format: yaml
  label: Truist Commercial Accounts
  slug: commercial-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-accounts-openapi.yml
- filename: bbandt-corp-commercial-account-balance-openapi.yml
  format: yaml
  label: Truist Commercial Account Balance
  slug: commercial-account-balance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-account-balance-openapi.yml
- filename: bbandt-corp-commercial-account-transactions-openapi.yml
  format: yaml
  label: Truist Commercial Account Transactions
  slug: commercial-account-transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-account-transactions-openapi.yml
- filename: bbandt-corp-retail-accounts-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Accounts
  slug: personal-small-business-accounts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-accounts-openapi.yml
- filename: bbandt-corp-retail-locator-openapi.yml
  format: yaml
  label: Truist Branch/ATM Locator
  slug: branch-atm-locator
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-locator-openapi.yml
- filename: bbandt-corp-retail-accounts-transaction-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Transactions
  slug: personal-small-business-transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-accounts-transaction-openapi.yml
- filename: bbandt-corp-retail-customers-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Client Contact
  slug: personal-and-small-business-client-contact
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-customers-openapi.yml
- filename: bbandt-corp-retail-auth-oauth-openapi.yml
  format: yaml
  label: Truist Retail Oauth Authentication
  slug: retail-oauth-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-auth-oauth-openapi.yml
- filename: bbandt-corp-retail-consents-openapi.yml
  format: yaml
  label: Truist User Consent
  slug: user-consent
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-consents-openapi.yml
- filename: bbandt-corp-retail-register-recipient-openapi.yml
  format: yaml
  label: Truist Retail Dynamic Client Registration
  slug: retail-dynamic-client-registration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-register-recipient-openapi.yml
- filename: bbandt-corp-retail-payment-networks-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Account Payment Networks
  slug: personal-and-small-business-account-payment-networks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-payment-networks-openapi.yml
- filename: bbandt-corp-retail-accounts-contact-openapi.yml
  format: yaml
  label: Truist Account Address
  slug: account-address
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-accounts-contact-openapi.yml
- filename: bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml
  format: yaml
  label: Truist Credit Transfers
  slug: credit-transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml
- filename: bbandt-corp-retail-event-notifications-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Event Notifications
  slug: personal-and-small-business-event-notifications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-event-notifications-openapi.yml
- filename: bbandt-corp-retail-event-subscriptions-openapi.yml
  format: yaml
  label: Truist Personal and Small Business Event Subscriptions
  slug: personal-and-small-business-event-subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/openapi/bbandt-corp-retail-event-subscriptions-openapi.yml
authorization_urls:
- https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/authorize
- https://api-sandbox.truist.com/commercial/auth/v1/oauth/authorize
- https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize
- https://api-sandbox.truist.com/retail-aggregator/auth/v1/oauth/authorize
description: ''
docs: https://developer.truist.com/api/retail-oauth-authentication/documentation
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Bbandt Corp Scopes
name_suffix: OAuth Scopes
note: Two scope vocabularies coexist. The retail (FDX) APIs use resource scopes — ACCOUNT_BASIC (account list), ACCOUNT_DETAILED (account detail), TRANSACTIONS, CUSTOMER_CONTACT, PAYMENT_SUPPORT — plus the standard OIDC scopes profile, email, phone and address. The commercial APIs use verb:resource scopes — read:accounts, read:payments, write:payments. Scope descriptions are taken verbatim from the specs; note that Truist swapped the descriptions of the email/phone/address OIDC scopes in retail-auth-oauth.yaml, which is a defect in their contract, not in this reading.
overview: 'BB&T Corp (Truist) publishes 12 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BB&T Corp (Truist) API on a user''s behalf.


  Tokens are issued from https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BB&T Corp (Truist)
provider_slug: bbandt-corp
schemes:
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/token
  name: OAuth
  source: openapi/bbandt-corp-commercial-account-balance-openapi.yml
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://api-sandbox.truist.com/commercial/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api-sandbox.truist.com/commercial/auth/v1/oauth/token
  name: OAuth
  source: openapi/bbandt-corp-commercial-account-transactions-openapi.yml
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/token
  name: OAuth
  source: openapi/bbandt-corp-commercial-accounts-openapi.yml
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://api-sandbox.truist.com/commercial/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api-sandbox.truist.com/commercial/auth/v2/oauth/token
  name: OAuth
  source: openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize
    flow: authorizationCode
    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token
  name: OAuth
  source: openapi/bbandt-corp-retail-accounts-contact-openapi.yml
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize
    flow: authorizationCode
    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token
  name: OAuth
  source: openapi/bbandt-corp-retail-accounts-openapi.yml
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize
    flow: authorizationCode
    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token
  name: OAuth
  source: openapi/bbandt-corp-retail-accounts-transaction-openapi.yml
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize
    flow: authorizationCode
    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token
  name: OAuth
  source: openapi/bbandt-corp-retail-auth-oauth-openapi.yml
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://api-sandbox.truist.com/retail-aggregator/auth/v1/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api-sandbox.truist.com/retail-aggregator/auth/v1/oauth/token
  name: OAuth
  source: openapi/bbandt-corp-retail-customers-openapi.yml
- description: The production authorization URL will be provided after the onboarding process is completed.
  flows:
  - authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize
    flow: authorizationCode
    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token
  name: OAuth
  source: openapi/bbandt-corp-retail-payment-networks-openapi.yml
scope_count: 12
scope_names:
- ACCOUNT_BASIC
- ACCOUNT_DETAILED
- CUSTOMER_CONTACT
- PAYMENT_SUPPORT
- TRANSACTIONS
- address
- email
- phone
- profile
- read:accounts
- read:payments
- write:payments
scopes:
- description: Scope required to access accountList
  flows:
  - authorizationCode
  scope: ACCOUNT_BASIC
- description: Scope required to access account details of accountId
  flows:
  - authorizationCode
  scope: ACCOUNT_DETAILED
- description: Scope required to access account contact
  flows:
  - authorizationCode
  scope: CUSTOMER_CONTACT
- description: Scope required to access payment networks supported by the account
  flows:
  - authorizationCode
  scope: PAYMENT_SUPPORT
- description: Scope required to access account transactions
  flows:
  - authorizationCode
  scope: TRANSACTIONS
- description: This scope value requests access to the email and email_verified Claims.
  flows:
  - authorizationCode
  scope: address
- description: This scope value requests access to the phone_number and phone_number_verified Claims.
  flows:
  - authorizationCode
  scope: email
- description: This scope value requests access to the address Claim
  flows:
  - authorizationCode
  scope: phone
- description: This scope value requests access to the End-User's default profile Claims, which are:name, family_name, given_name, middle_name, zoneinfo, locale, and updated_at.
  flows:
  - authorizationCode
  scope: profile
- description: Scope is requied to access account balance data
  flows:
  - authorizationCode
  scope: read:accounts
- description: Scope required to read payment details
  flows:
  - authorizationCode
  scope: read:payments
- description: Scope required to create or update payments
  flows:
  - authorizationCode
  scope: write:payments
slug: bbandt-corp-scopes
source_filename: bbandt-corp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/bbandt-corp-commercial-account-balance-openapi.yml, openapi/bbandt-corp-commercial-account-transactions-openapi.yml,\n  openapi/bbandt-corp-commercial-accounts-openapi.yml, openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml,\n  openapi/bbandt-corp-retail-accounts-contact-openapi.yml, openapi/bbandt-corp-retail-accounts-openapi.yml, openapi/bbandt-corp-retail-accounts-transaction-openapi.yml,\n  openapi/bbandt-corp-retail-auth-oauth-openapi.yml, openapi/bbandt-corp-retail-customers-openapi.yml, openapi/bbandt-corp-retail-payment-networks-openapi.yml\nschemes:\n- name: OAuth\n  source: openapi/bbandt-corp-commercial-account-balance-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/authorize\n    tokenUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/token\n  description: The production authorization URL will\
  \ be provided after the onboarding process is completed.\n- name: OAuth\n  source: openapi/bbandt-corp-commercial-account-transactions-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-sandbox.truist.com/commercial/auth/v1/oauth/authorize\n    tokenUrl: https://api-sandbox.truist.com/commercial/auth/v1/oauth/token\n  description: The production authorization URL will be provided after the onboarding process is completed.\n- name: OAuth\n  source: openapi/bbandt-corp-commercial-accounts-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/authorize\n    tokenUrl: https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/token\n  description: The production authorization URL will be provided after the onboarding process is completed.\n- name: OAuth\n  source: openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://api-sandbox.truist.com/commercial/auth/v1/oauth/authorize\n    tokenUrl: https://api-sandbox.truist.com/commercial/auth/v2/oauth/token\n  description: The production authorization URL will be provided after the onboarding process is completed.\n- name: OAuth\n  source: openapi/bbandt-corp-retail-accounts-contact-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize\n    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token\n  description: The production authorization URL will be provided after the onboarding process is completed.\n- name: OAuth\n  source: openapi/bbandt-corp-retail-accounts-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize\n    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token\n  description: The production authorization URL will be provided after the onboarding\
  \ process is completed.\n- name: OAuth\n  source: openapi/bbandt-corp-retail-accounts-transaction-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize\n    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token\n  description: The production authorization URL will be provided after the onboarding process is completed.\n- name: OAuth\n  source: openapi/bbandt-corp-retail-auth-oauth-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize\n    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token\n  description: The production authorization URL will be provided after the onboarding process is completed.\n- name: OAuth\n  source: openapi/bbandt-corp-retail-customers-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-sandbox.truist.com/retail-aggregator/auth/v1/oauth/authorize\n\
  \    tokenUrl: https://api-sandbox.truist.com/retail-aggregator/auth/v1/oauth/token\n  description: The production authorization URL will be provided after the onboarding process is completed.\n- name: OAuth\n  source: openapi/bbandt-corp-retail-payment-networks-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/authorize\n    tokenUrl: https://api-sandbox.truist.com/retail/auth/oauth/v3/token\n  description: The production authorization URL will be provided after the onboarding process is completed.\nscopes:\n- scope: ACCOUNT_BASIC\n  description: Scope required to access accountList\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-retail-accounts-openapi.yml\n- scope: ACCOUNT_DETAILED\n  description: Scope required to access account details of accountId\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-retail-accounts-openapi.yml\n- scope: CUSTOMER_CONTACT\n  description:\
  \ Scope required to access account contact\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-retail-accounts-contact-openapi.yml\n  - openapi/bbandt-corp-retail-customers-openapi.yml\n- scope: PAYMENT_SUPPORT\n  description: Scope required to access payment networks supported by the account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-retail-payment-networks-openapi.yml\n- scope: TRANSACTIONS\n  description: Scope required to access account transactions\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-retail-accounts-transaction-openapi.yml\n- scope: address\n  description: This scope value requests access to the email and email_verified Claims.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-retail-auth-oauth-openapi.yml\n- scope: email\n  description: This scope value requests access to the phone_number and phone_number_verified Claims.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-retail-auth-oauth-openapi.yml\n\
  - scope: phone\n  description: This scope value requests access to the address Claim\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-retail-auth-oauth-openapi.yml\n- scope: profile\n  description: This scope value requests access to the End-User's default profile Claims, which are:name, family_name,\n    given_name, middle_name, zoneinfo, locale, and updated_at.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-retail-auth-oauth-openapi.yml\n- scope: read:accounts\n  description: Scope is requied to access account balance data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-commercial-account-balance-openapi.yml\n  - openapi/bbandt-corp-commercial-account-transactions-openapi.yml\n  - openapi/bbandt-corp-commercial-accounts-openapi.yml\n  - openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml\n- scope: read:payments\n  description: Scope required to read payment details\n  flows:\n  - authorizationCode\n  sources:\n\
  \  - openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml\n- scope: write:payments\n  description: Scope required to create or update payments\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/bbandt-corp-commercial-credit-transfers-oas-v2-openapi.yml\ndocs: https://developer.truist.com/api/retail-oauth-authentication/documentation\nnote: Two scope vocabularies coexist. The retail (FDX) APIs use resource scopes — ACCOUNT_BASIC (account list), ACCOUNT_DETAILED\n  (account detail), TRANSACTIONS, CUSTOMER_CONTACT, PAYMENT_SUPPORT — plus the standard OIDC scopes profile, email, phone\n  and address. The commercial APIs use verb:resource scopes — read:accounts, read:payments, write:payments. Scope descriptions\n  are taken verbatim from the specs; note that Truist swapped the descriptions of the email/phone/address OIDC scopes\n  in retail-auth-oauth.yaml, which is a defect in their contract, not in this reading.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bbandt-corp/refs/heads/main/scopes/bbandt-corp-scopes.yml
summary_line: 12 scopes · authorizationCode
tags:
- Banking
- Financial-Services
- Open Banking
- Truist
- BB&T
- Fortune 500
token_urls:
- https://apidev-sandbox.truist.com/commercial/auth/v1/oauth/token
- https://api-sandbox.truist.com/commercial/auth/v1/oauth/token
- https://api-sandbox.truist.com/commercial/auth/v2/oauth/token
- https://api-sandbox.truist.com/retail/auth/oauth/v3/token
- https://api-sandbox.truist.com/retail-aggregator/auth/v1/oauth/token
---
