---
api_specs:
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Payment Intent API
  slug: ziina-payment-intent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Refund API
  slug: ziina-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Transfer API
  slug: ziina-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Webhooks API
  slug: ziina-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
- filename: ziina-openapi.yml
  format: yaml
  label: Ziina Account API
  slug: ziina-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/openapi/ziina-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.ziina.com/developers/oauth-2.0#available-scopes
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Ziina Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Ziina publishes 7 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Ziina API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Ziina
provider_slug: ziina
schemes:
- authorizationUrl: https://auth.ziina.com/oidc/auth
  flow: authorizationCode
  grantTypes:
  - authorization_code
  - refresh_token
  - client_credentials
  - implicit
  issuer: https://auth.ziina.com
  name: oauth2
  pkce:
  - S256
  sources:
  - https://docs.ziina.com/developers/oauth-2.0
  - well-known/ziina-openid-configuration.json
  tokenUrl: https://auth.ziina.com/oidc/token
  type: oauth2
scope_count: 7
scope_names:
- read_account
- write_payment_intents
- write_refunds
- write_transfers
- write_webhooks
- offline_access
- openid
scopes:
- description: Read the connected account profile (GET /account) - account_id, type, status, ziiname, display_name.
  flows:
  - authorizationCode
  scope: read_account
- description: Create payment intents and accept payments on the account's behalf.
  flows:
  - authorizationCode
  scope: write_payment_intents
- description: Create and fetch refunds against payment intents.
  flows:
  - authorizationCode
  scope: write_refunds
- description: Transfer money to other Ziina users.
  flows:
  - authorizationCode
  scope: write_transfers
- description: Register and delete webhook endpoints.
  flows:
  - authorizationCode
  scope: write_webhooks
- description: Issue a refresh_token for long-lived access (requires prompt=consent on the authorization request).
  flows:
  - authorizationCode
  scope: offline_access
- description: OIDC base scope; returns an ID token identifying the end user.
  flows:
  - authorizationCode
  scope: openid
slug: ziina-scopes
source_filename: ziina-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/ziina-openapi.yml\ndocs: https://docs.ziina.com/developers/oauth-2.0#available-scopes\nwell_known: well-known/ziina-openid-configuration.json\nnotes: >-\n  The published OpenAPI declares only an HTTP bearer (JWT) security scheme, so no\n  scopes are derivable from the spec alone. Ziina documents an OIDC-based OAuth\n  2.0 authorization server (auth.ziina.com/oidc); the scopes below are captured\n  verbatim from the docs' \"Available scopes\" reference and confirmed against the\n  live OIDC discovery document's scopes_supported list. Multiple scopes are\n  requested joined by a \"+\" sign. Tokens minted on the Ziina business connect\n  page (https://ziina.com/business/connect) carry all available scopes.\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  issuer: https://auth.ziina.com\n  authorizationUrl: https://auth.ziina.com/oidc/auth\n  tokenUrl: https://auth.ziina.com/oidc/token\n  grantTypes:\n\
  \  - authorization_code\n  - refresh_token\n  - client_credentials\n  - implicit\n  pkce: [S256]\n  sources:\n  - https://docs.ziina.com/developers/oauth-2.0\n  - well-known/ziina-openid-configuration.json\nscopes:\n- scope: read_account\n  description: Read the connected account profile (GET /account) - account_id, type, status, ziiname, display_name.\n  flows: [authorizationCode]\n- scope: write_payment_intents\n  description: Create payment intents and accept payments on the account's behalf.\n  flows: [authorizationCode]\n- scope: write_refunds\n  description: Create and fetch refunds against payment intents.\n  flows: [authorizationCode]\n- scope: write_transfers\n  description: Transfer money to other Ziina users.\n  flows: [authorizationCode]\n- scope: write_webhooks\n  description: Register and delete webhook endpoints.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issue a refresh_token for long-lived access (requires prompt=consent on the authorization\
  \ request).\n  flows: [authorizationCode]\n- scope: openid\n  description: OIDC base scope; returns an ID token identifying the end user.\n  flows: [authorizationCode]\n  source: well-known/ziina-openid-configuration.json\noidc_extra_scopes_advertised:\n- profile\n- email\n- phone\n- address\n- write_pos_sessions\n- write_api_keys\noidc_extra_note: >-\n  The live OIDC discovery scopes_supported and claims_supported also advertise\n  write_pos_sessions and write_api_keys (plus standard OIDC profile/email/phone/\n  address). These are not listed in the public developer scope reference and may\n  be reserved for first-party or POS integrations; documented here for\n  completeness.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ziina/refs/heads/main/scopes/ziina-scopes.yml
summary_line: 7 scopes
tags:
- Payments
- Fintech
- UAE
- MENA
- Money Transfer
- Wallet
token_urls: []
---
