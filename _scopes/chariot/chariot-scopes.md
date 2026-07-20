---
api_specs:
- filename: chariot-openapi-original.yml
  format: yaml
  label: Chariot API
  slug: chariot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chariot/refs/heads/main/openapi/chariot-openapi-original.yml
- filename: chariot-fdx-openapi-original.yml
  format: yaml
  label: Chariot FDX API
  slug: chariot-fdx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chariot/refs/heads/main/openapi/chariot-fdx-openapi-original.yml
authorization_urls:
- https://dashboard.givechariot.com/oauth/authorize
description: ''
docs: https://docs.givechariot.com/api/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Chariot Scopes
name_suffix: OAuth Scopes
note: The two FDX scopes are mutually exclusive per authorization. OIDC discovery (/.well-known/openid-configuration) additionally advertises openid and offline_access, and grant types authorization_code, refresh_token, client_credentials, and token-exchange.
overview: 'Chariot publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Chariot API on a user''s behalf.


  Tokens are issued from https://api.givechariot.com/auth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Chariot
provider_slug: chariot
schemes:
- description: OAuth 2.0 Bearer token. A client may hold both scopes, but each FDX authorization must contain exactly one — they are mutually exclusive per authorization. An authorization containing both will be rejected. See the Authentication page for token exchange details.
  flows:
  - authorizationUrl: https://dashboard.givechariot.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.givechariot.com/auth/oauth/token
  name: oauth2
  source: openapi/chariot-fdx-openapi-original.yml
scope_count: 4
scope_names:
- read:bank_accounts
- sync:connected_accounts
- openid
- offline_access
scopes:
- description: Read access to bank account data
  flows:
  - authorizationCode
  scope: read:bank_accounts
- description: Sync access to connected account data
  flows:
  - authorizationCode
  scope: sync:connected_accounts
- description: OpenID Connect authentication (present in OIDC discovery scopes_supported).
  flows: []
  scope: openid
- description: Request a refresh token for long-lived access (present in OIDC discovery scopes_supported).
  flows: []
  scope: offline_access
slug: chariot-scopes
source_filename: chariot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/chariot-fdx-openapi-original.yml, well-known/chariot-openid-configuration.json\ndocs: https://docs.givechariot.com/api/authentication\nschemes:\n- name: oauth2\n  source: openapi/chariot-fdx-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dashboard.givechariot.com/oauth/authorize\n    tokenUrl: https://api.givechariot.com/auth/oauth/token\n  description: OAuth 2.0 Bearer token. A client may hold both scopes, but each FDX authorization\n    must contain exactly one — they are mutually exclusive per authorization. An authorization\n    containing both will be rejected. See the Authentication page for token exchange details.\nscopes:\n- scope: read:bank_accounts\n  description: Read access to bank account data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chariot-fdx-openapi-original.yml\n- scope: sync:connected_accounts\n  description: Sync access to connected account\
  \ data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/chariot-fdx-openapi-original.yml\n- scope: openid\n  description: OpenID Connect authentication (present in OIDC discovery scopes_supported).\n  sources:\n  - well-known/chariot-openid-configuration.json\n- scope: offline_access\n  description: Request a refresh token for long-lived access (present in OIDC discovery scopes_supported).\n  sources:\n  - well-known/chariot-openid-configuration.json\nnote: >-\n  The two FDX scopes are mutually exclusive per authorization. OIDC discovery\n  (/.well-known/openid-configuration) additionally advertises openid and offline_access, and grant\n  types authorization_code, refresh_token, client_credentials, and token-exchange.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chariot/refs/heads/main/scopes/chariot-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Payments
- Donor Advised Funds
- Charitable Giving
- Nonprofit
- Fintech
- DAFpay
- Grants
- Disbursements
- Open Banking
- FDX
- Webhooks
- Company
token_urls:
- https://api.givechariot.com/auth/oauth/token
---
