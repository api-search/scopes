---
api_specs:
- filename: zepto-payments-zepto.yml
  format: yaml
  label: Zepto API
  slug: zepto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-zepto.yml
- filename: zepto-payments-pay-to.yml
  format: yaml
  label: Zepto PayTo API
  slug: payto-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-pay-to.yml
- filename: zepto-payments-validate-cop.yml
  format: yaml
  label: Zepto Validate API (Confirmation of Payee)
  slug: validate-cop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-validate-cop.yml
- filename: zepto-payments-investigations.yml
  format: yaml
  label: Zepto Investigations API
  slug: investigations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-investigations.yml
- filename: zepto-payments-clients.yml
  format: yaml
  label: Zepto Clients API
  slug: clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-clients.yml
- filename: zepto-payments-merchant-reports.yml
  format: yaml
  label: Zepto Merchant Reports API
  slug: merchant-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-merchant-reports.yml
- filename: zepto-payments-notifications.yml
  format: yaml
  label: Zepto Notifications API (Webhooks)
  slug: notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/openapi/zepto-payments-notifications.yml
authorization_urls:
- /oauth/authorize
description: ''
docs: https://docs.zeptopayments.com/docs/oauth-grant-flow
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Zepto Payments Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Zepto publishes 9 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Zepto API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Zepto
provider_slug: zepto-payments
schemes:
- flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: bearerAuth
  source: openapi/zepto-payments-zepto.yml
scope_count: 9
scope_names:
- agreements
- contacts
- open_agreements
- payment_requests
- payments
- public
- refunds
- transactions
- transfers
scopes:
- description: Manage your agreements
  flows:
  - authorizationCode
  scope: agreements
- description: Manage your contacts
  flows:
  - authorizationCode
  scope: contacts
- description: Manage your open agreements
  flows:
  - authorizationCode
  scope: open_agreements
- description: Manage your payment requests
  flows:
  - authorizationCode
  scope: payment_requests
- description: Manage your payments
  flows:
  - authorizationCode
  scope: payments
- description: Access your public information
  flows:
  - authorizationCode
  scope: public
- description: Manage your refunds
  flows:
  - authorizationCode
  scope: refunds
- description: Access your transaction history
  flows:
  - authorizationCode
  scope: transactions
- description: Manage your Transfers
  flows:
  - authorizationCode
  scope: transfers
slug: zepto-payments-scopes
source_filename: zepto-payments-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: searched\nsource: openapi/zepto-payments-zepto.yml\ndocs: https://docs.zeptopayments.com/docs/oauth-grant-flow\nschemes:\n- name: bearerAuth\n  source: openapi/zepto-payments-zepto.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\nscopes:\n- scope: agreements\n  description: Manage your agreements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zepto-payments-zepto.yml\n- scope: contacts\n  description: Manage your contacts\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zepto-payments-zepto.yml\n- scope: open_agreements\n  description: Manage your open agreements\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zepto-payments-zepto.yml\n- scope: payment_requests\n  description: Manage your payment requests\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zepto-payments-zepto.yml\n- scope: payments\n  description: Manage your payments\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/zepto-payments-zepto.yml\n- scope: public\n  description: Access your public information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zepto-payments-zepto.yml\n- scope: refunds\n  description: Manage your refunds\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zepto-payments-zepto.yml\n- scope: transactions\n  description: Access your transaction history\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zepto-payments-zepto.yml\n- scope: transfers\n  description: Manage your Transfers\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/zepto-payments-zepto.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zepto-payments/refs/heads/main/scopes/zepto-payments-scopes.yml
summary_line: 9 scopes · authorizationCode
tags:
- Payments
- Australia
- Real-Time Payments
- Account-to-Account
- New Payments Platform
- PayTo
- PayID
- Direct Entry
- Open Banking
- Money Movement
token_urls:
- /oauth/token
---
