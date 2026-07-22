---
api_specs:
- filename: coinme-caas-openapi.json
  format: json
  label: Coinme Crypto-as-a-Service API
  slug: coinme-crypto-as-a-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coinme/refs/heads/main/openapi/coinme-caas-openapi.json
authorization_urls: []
description: ''
docs: https://auth.coinme.com/.well-known/openid-configuration
flows:
- authorization_code
- refresh_token
- client_credentials
- device_code
kind: oauth-scopes
layout: scope
method: searched
name: Coinme Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Coinme publishes 3 OAuth 2.0 scopes via the authorization_code, refresh_token, client_credentials, and device_code flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coinme API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coinme
provider_slug: coinme
schemes:
- authorizationUrl: https://auth.coinme.com/oauth/authorize
  flows:
  - authorization_code
  - refresh_token
  - client_credentials
  - device_code
  name: OIDC
  source: https://auth.coinme.com/.well-known/openid-configuration
  tokenUrl: https://auth.coinme.com/oauth/token
scope_count: 3
scope_names:
- openid
- profile
- email
scopes:
- description: OIDC authentication; issue an ID token for the authenticated Coinme user.
  flows: []
  scope: openid
- description: Access the user's basic profile claims.
  flows: []
  scope: profile
- description: Access the user's email address.
  flows: []
  scope: email
slug: coinme-scopes
source_filename: coinme-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.coinme.com/.well-known/openid-configuration\ndocs: https://auth.coinme.com/.well-known/openid-configuration\nnotes: >-\n  The partner Crypto-as-a-Service API (caas.coinme.com) authenticates with HTTP Basic + x-api-key\n  and declares no OAuth2 scopes. These scopes belong to the separate Coinme consumer OIDC provider\n  at auth.coinme.com, captured from its published discovery document. Grants supported:\n  authorization_code, refresh_token, client_credentials, token-exchange, device_code.\nschemes:\n- name: OIDC\n  source: https://auth.coinme.com/.well-known/openid-configuration\n  authorizationUrl: https://auth.coinme.com/oauth/authorize\n  tokenUrl: https://auth.coinme.com/oauth/token\n  flows:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - device_code\nscopes:\n- scope: openid\n  description: OIDC authentication; issue an ID token for the authenticated Coinme user.\n- scope: profile\n\
  \  description: Access the user's basic profile claims.\n- scope: email\n  description: Access the user's email address.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coinme/refs/heads/main/scopes/coinme-scopes.yml
summary_line: 3 scopes · authorization_code/refresh_token/client_credentials/device_code
tags:
- Company
- Crypto
- Cryptocurrency
- Payments
- Bitcoin
- Wallet
- KYC
- Onboarding
- Fintech
- Crypto-as-a-Service
- On-Ramp
- Off-Ramp
token_urls: []
---
