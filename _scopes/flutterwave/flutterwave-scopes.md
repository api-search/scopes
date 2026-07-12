---
authorization_urls: []
description: ''
docs: https://developer.flutterwave.com/docs/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Flutterwave Scopes
name_suffix: OAuth Scopes
note: Flutterwave's v4 API uses OAuth 2.0 client_credentials (client_id/client_secret via idp.flutterwave.com) without documented API permission scopes; token responses only carry default OIDC scopes such as "profile email" (https://developer.flutterwave.com/docs/authentication).
overview: 'Flutterwave uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flutterwave
provider_slug: flutterwave
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token
  name: OAuth2
  source: openapi/flutterwave-banks-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token
  name: OAuth2
  source: openapi/flutterwave-payments-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token
  name: OAuth2
  source: openapi/flutterwave-settlements-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token
  name: OAuth2
  source: openapi/flutterwave-transfers-api-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token
  name: OAuth2
  source: openapi/flutterwave-wallets-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: flutterwave-scopes
source_filename: flutterwave-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/flutterwave-banks-api-openapi.yml, openapi/flutterwave-payments-api-openapi.yml,\n  openapi/flutterwave-settlements-api-openapi.yml, openapi/flutterwave-transfers-api-openapi.yml,\n  openapi/flutterwave-wallets-api-openapi.yml\ndocs: https://developer.flutterwave.com/docs/authentication\nnote: Flutterwave's v4 API uses OAuth 2.0 client_credentials (client_id/client_secret\n  via idp.flutterwave.com) without documented API permission scopes; token responses\n  only carry default OIDC scopes such as \"profile email\"\n  (https://developer.flutterwave.com/docs/authentication).\nschemes:\n- name: OAuth2\n  source: openapi/flutterwave-banks-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token\n- name: OAuth2\n  source: openapi/flutterwave-payments-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token\n\
  - name: OAuth2\n  source: openapi/flutterwave-settlements-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token\n- name: OAuth2\n  source: openapi/flutterwave-transfers-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token\n- name: OAuth2\n  source: openapi/flutterwave-wallets-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flutterwave/refs/heads/main/scopes/flutterwave-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Payments
- Payouts
- Mobile Money
- Cards
- Africa
- Fintech
- Remittance
- Virtual Accounts
- Chargebacks
- Multi-Currency
token_urls:
- https://idp.flutterwave.com/realms/flutterwave/protocol/openid-connect/token
---
