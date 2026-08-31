---
api_specs:
- filename: mercado-pago-asyncapi.yml
  format: yaml
  label: Mercado Pago Webhooks / Notifications
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/asyncapi/mercado-pago-asyncapi.yml
- filename: mercado-pago-authentication-api-openapi.yml
  format: yaml
  label: Mercado Pago Authentication API
  slug: mercado-pago-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-authentication-api-openapi.yml
- filename: mercado-pago-cards-api-openapi.yml
  format: yaml
  label: Mercado Pago Cards API
  slug: mercado-pago-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-cards-api-openapi.yml
- filename: mercado-pago-chargebacks-api-openapi.yml
  format: yaml
  label: Mercado Pago Chargebacks API
  slug: mercado-pago-chargebacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-chargebacks-api-openapi.yml
- filename: mercado-pago-claims-api-openapi.yml
  format: yaml
  label: Mercado Pago Claims API
  slug: mercado-pago-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-claims-api-openapi.yml
- filename: mercado-pago-customers-api-openapi.yml
  format: yaml
  label: Mercado Pago Customers API
  slug: mercado-pago-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-customers-api-openapi.yml
- filename: mercado-pago-merchant-orders-api-openapi.yml
  format: yaml
  label: Mercado Pago Merchant Orders API
  slug: mercado-pago-merchant-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-merchant-orders-api-openapi.yml
- filename: mercado-pago-orders-api-openapi.yml
  format: yaml
  label: Mercado Pago Orders API
  slug: mercado-pago-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-orders-api-openapi.yml
- filename: mercado-pago-payment-methods-api-openapi.yml
  format: yaml
  label: Mercado Pago Payment Methods API
  slug: mercado-pago-payment-methods-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-payment-methods-api-openapi.yml
- filename: mercado-pago-payments-api-openapi.yml
  format: yaml
  label: Mercado Pago Payments API
  slug: mercado-pago-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-payments-api-openapi.yml
- filename: mercado-pago-plans-api-openapi.yml
  format: yaml
  label: Mercado Pago Plans API
  slug: mercado-pago-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-plans-api-openapi.yml
- filename: mercado-pago-point-api-openapi.yml
  format: yaml
  label: Mercado Pago Point API
  slug: mercado-pago-point-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-point-api-openapi.yml
- filename: mercado-pago-preferences-api-openapi.yml
  format: yaml
  label: Mercado Pago Preferences API
  slug: mercado-pago-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-preferences-api-openapi.yml
- filename: mercado-pago-qr-api-openapi.yml
  format: yaml
  label: Mercado Pago QR API
  slug: mercado-pago-qr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-qr-api-openapi.yml
- filename: mercado-pago-refunds-api-openapi.yml
  format: yaml
  label: Mercado Pago Refunds API
  slug: mercado-pago-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-refunds-api-openapi.yml
- filename: mercado-pago-reports-api-openapi.yml
  format: yaml
  label: Mercado Pago Reports API
  slug: mercado-pago-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-reports-api-openapi.yml
- filename: mercado-pago-subscriptions-api-openapi.yml
  format: yaml
  label: Mercado Pago Subscriptions API
  slug: mercado-pago-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-subscriptions-api-openapi.yml
authorization_urls:
- https://auth.mercadopago.com/authorization
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Mercado Pago Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mercado Pago publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mercado Pago API on a user''s behalf.


  Tokens are issued from https://api.mercadopago.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mercado Pago
provider_slug: mercado-pago
schemes:
- flows:
  - authorizationUrl: https://auth.mercadopago.com/authorization
    flow: authorizationCode
    tokenUrl: https://api.mercadopago.com/oauth/token
  name: oauth2
  source: openapi/mercado-pago-openapi.yml
scope_count: 3
scope_names:
- offline_access
- read
- write
scopes:
- description: Persistent refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: Read merchant data
  flows:
  - authorizationCode
  scope: read
- description: Write merchant data
  flows:
  - authorizationCode
  scope: write
slug: mercado-pago-scopes
source_filename: mercado-pago-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mercado-pago-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/mercado-pago-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mercadopago.com/authorization\n    tokenUrl: https://api.mercadopago.com/oauth/token\nscopes:\n- scope: offline_access\n  description: Persistent refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mercado-pago-openapi.yml\n- scope: read\n  description: Read merchant data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mercado-pago-openapi.yml\n- scope: write\n  description: Write merchant data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mercado-pago-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/scopes/mercado-pago-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Payments
- Checkout
- Subscription
- POS
- QR
- PIX
- SDK
- Wallets
- Acquiring
- Lending
- Issuing
- Latin America
- Brazil
- Argentina
- Mexico
- Chile
- Colombia
- Peru
- Uruguay
- Fintech
token_urls:
- https://api.mercadopago.com/oauth/token
---
