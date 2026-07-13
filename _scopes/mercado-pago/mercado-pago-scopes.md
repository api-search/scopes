---
api_specs:
- filename: mercado-pago-openapi.yml
  format: yaml
  label: Mercado Pago Payments API
  slug: payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/openapi/mercado-pago-openapi.yml
- filename: mercado-pago-asyncapi.yml
  format: yaml
  label: Mercado Pago Webhooks / Notifications
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercado-pago/refs/heads/main/asyncapi/mercado-pago-asyncapi.yml
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
- Subscriptions
- POS
- QR
- PIX
- SDKs
- Wallet
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
