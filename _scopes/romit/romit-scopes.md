---
api_specs:
- filename: romit-openapi.yml
  format: yaml
  label: Romit API
  slug: romit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/openapi/romit-openapi.yml
authorization_urls:
- https://api.romit.io/v1/oauth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Romit Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Romit publishes 15 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Romit API on a user''s behalf.


  Tokens are issued from https://api.romit.io/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Romit
provider_slug: romit
schemes:
- description: Romit used OAuth2. User-context flows (authorization_code / refresh_token) authorize a customer against requested scopes; the client_credentials flow issues an application access token. Access tokens are presented as an HTTP Bearer token.
  flows:
  - authorizationUrl: https://api.romit.io/v1/oauth
    flow: authorizationCode
    tokenUrl: https://api.romit.io/v1/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.romit.io/v1/oauth/token
  name: oauth2
  source: openapi/romit-openapi.yml
scope_count: 15
scope_names:
- BANKING_READ
- BANKING_WRITE
- DEFAULT
- IDENTITY_READ
- IDENTITY_WRITE
- INVOICE_READ
- INVOICE_WRITE
- PLAN_READ
- PLAN_WRITE
- SUBSCRIPTION_READ
- SUBSCRIPTION_WRITE
- TRANSFER_READ
- TRANSFER_WRITE
- USER_READ
- USER_WRITE
scopes:
- description: Read access to Banking
  flows:
  - authorizationCode
  scope: BANKING_READ
- description: Write access to Banking
  flows:
  - authorizationCode
  scope: BANKING_WRITE
- description: Access to basic information
  flows:
  - authorizationCode
  - clientCredentials
  scope: DEFAULT
- description: Read access to Identity
  flows:
  - authorizationCode
  scope: IDENTITY_READ
- description: Write access to Identity
  flows:
  - authorizationCode
  scope: IDENTITY_WRITE
- description: Read access to Invoice
  flows:
  - authorizationCode
  scope: INVOICE_READ
- description: Write access to Invoice
  flows:
  - authorizationCode
  scope: INVOICE_WRITE
- description: Read access to Plan
  flows:
  - authorizationCode
  scope: PLAN_READ
- description: Write access to Plan
  flows:
  - authorizationCode
  scope: PLAN_WRITE
- description: Read access to Subscription
  flows:
  - authorizationCode
  scope: SUBSCRIPTION_READ
- description: Write access to Subscription
  flows:
  - authorizationCode
  scope: SUBSCRIPTION_WRITE
- description: Read access to Transfer
  flows:
  - authorizationCode
  scope: TRANSFER_READ
- description: Write access to Transfer
  flows:
  - authorizationCode
  scope: TRANSFER_WRITE
- description: Read access to User
  flows:
  - authorizationCode
  scope: USER_READ
- description: Write access to User
  flows:
  - authorizationCode
  scope: USER_WRITE
slug: romit-scopes
source_filename: romit-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/romit-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/romit-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.romit.io/v1/oauth\n    tokenUrl: https://api.romit.io/v1/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.romit.io/v1/oauth/token\n  description: Romit used OAuth2. User-context flows (authorization_code / refresh_token) authorize\n    a customer against requested scopes; the client_credentials flow issues an application access\n    token. Access tokens are presented as an HTTP Bearer token.\nscopes:\n- scope: BANKING_READ\n  description: Read access to Banking\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: BANKING_WRITE\n  description: Write access to Banking\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: DEFAULT\n  description: Access to basic information\n  flows:\n\
  \  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/romit-openapi.yml\n- scope: IDENTITY_READ\n  description: Read access to Identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: IDENTITY_WRITE\n  description: Write access to Identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: INVOICE_READ\n  description: Read access to Invoice\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: INVOICE_WRITE\n  description: Write access to Invoice\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: PLAN_READ\n  description: Read access to Plan\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: PLAN_WRITE\n  description: Write access to Plan\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: SUBSCRIPTION_READ\n  description: Read access to Subscription\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: SUBSCRIPTION_WRITE\n  description: Write access to Subscription\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: TRANSFER_READ\n  description: Read access to Transfer\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: TRANSFER_WRITE\n  description: Write access to Transfer\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: USER_READ\n  description: Read access to User\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n- scope: USER_WRITE\n  description: Write access to User\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/romit-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/romit/refs/heads/main/scopes/romit-scopes.yml
summary_line: 15 scopes · authorizationCode/clientCredentials
tags:
- Company
- Payments
- Fintech
- Digital Wallet
- Payment Gateway
- Merchant Services
- Chargebacks
- Fraud Prevention
- Invoicing
- Subscriptions
token_urls:
- https://api.romit.io/v1/oauth/token
---
