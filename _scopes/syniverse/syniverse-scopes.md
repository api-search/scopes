---
api_specs:
- filename: syniverse-omni-channel-messaging-openapi.yml
  format: yaml
  label: Syniverse Omni-Channel Messaging API (SCG)
  slug: syniverse-omni-channel-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-omni-channel-messaging-openapi.yml
- filename: syniverse-multi-factor-authentication-openapi.yml
  format: yaml
  label: Syniverse Multi-Factor Authentication API
  slug: syniverse-multi-factor-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-multi-factor-authentication-openapi.yml
- filename: syniverse-phone-number-verification-openapi.yml
  format: yaml
  label: Syniverse Phone Number Verification API
  slug: syniverse-phone-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-phone-number-verification-openapi.yml
- filename: syniverse-right-party-verification-openapi.yml
  format: yaml
  label: Syniverse Right Party Verification API
  slug: syniverse-right-party-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-right-party-verification-openapi.yml
- filename: syniverse-account-takeover-detection-openapi.yml
  format: yaml
  label: Syniverse Account Takeover Detection API
  slug: syniverse-account-takeover-detection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-account-takeover-detection-openapi.yml
- filename: syniverse-messaging-trust-resolve-openapi.yml
  format: yaml
  label: Syniverse Messaging Trust Resolve API
  slug: syniverse-messaging-trust-resolve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-messaging-trust-resolve-openapi.yml
- filename: syniverse-messaging-trust-datafeed-openapi.yml
  format: yaml
  label: Syniverse Messaging Trust Spam Datafeed API
  slug: syniverse-messaging-trust-spam-datafeed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-messaging-trust-datafeed-openapi.yml
- filename: syniverse-10dlc-openapi.yml
  format: yaml
  label: Syniverse 10DLC API
  slug: syniverse-10dlc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-10dlc-openapi.yml
- filename: syniverse-10dlc-number-pool-openapi.yml
  format: yaml
  label: Syniverse 10DLC Number Pool API (v1, deprecated)
  slug: syniverse-10dlc-number-pool-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-10dlc-number-pool-openapi.yml
- filename: syniverse-whitelisting-service-openapi.json
  format: json
  label: Syniverse Whitelisting Service API
  slug: syniverse-whitelisting-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-whitelisting-service-openapi.json
- filename: syniverse-token-management-openapi.yml
  format: yaml
  label: Syniverse SDC Application Access Token Management API
  slug: syniverse-access-token-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/openapi/syniverse-token-management-openapi.yml
authorization_urls:
- https://beta.api.syniverse.com/token
description: ''
docs: ''
flows:
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Syniverse Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Syniverse uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.mt1.messaging-trust.syniverse.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Syniverse
provider_slug: syniverse
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.mt1.messaging-trust.syniverse.com/oauth2/token
  name: OAuth2
  source: openapi/syniverse-messaging-trust-datafeed-openapi.yml
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.mt1.messaging-trust.syniverse.com/oauth2/token
  name: OAuth2
  source: openapi/syniverse-messaging-trust-resolve-openapi.yml
- flows:
  - authorizationUrl: https://beta.api.syniverse.com/token
    flow: implicit
  name: default
  source: openapi/syniverse-whitelisting-service-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: syniverse-scopes
source_filename: syniverse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: derived\nsource: openapi/syniverse-messaging-trust-datafeed-openapi.yml, openapi/syniverse-messaging-trust-resolve-openapi.yml,\n  openapi/syniverse-whitelisting-service-openapi.json\nsummary: >-\n  Syniverse declares three oauth2 security schemes but publishes ZERO scopes. Every flow\n  carries an empty scopes map, no operation names a scope in its security requirement, and\n  the Developer Community documentation has no scopes or permissions reference page — the\n  docs and support knowledge base were searched on 2026-07-25 and none exists. Authorization\n  is coarse: an SDC application access token carries whatever entitlements the account\n  holds, and 403 Forbidden means \"credentials do not carry the entitlements\" rather than\n  \"missing scope\". Recorded as a genuine empty result, not a gap in the harvest.\nscopes_documented: false\ndocs: null\nschemes:\n- name: OAuth2\n  source: openapi/syniverse-messaging-trust-datafeed-openapi.yml\n\
  \  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.mt1.messaging-trust.syniverse.com/oauth2/token\n- name: OAuth2\n  source: openapi/syniverse-messaging-trust-resolve-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.mt1.messaging-trust.syniverse.com/oauth2/token\n- name: default\n  source: openapi/syniverse-whitelisting-service-openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://beta.api.syniverse.com/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syniverse/refs/heads/main/scopes/syniverse-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Telecommunications
- United States
- CPaaS
- Messaging
- SMS
- Roaming
- IPX
- Wholesale
- Identity Verification
- SIM Swap
- 10DLC
- Open Gateway
- Network APIs
- Aggregator
token_urls:
- https://api.mt1.messaging-trust.syniverse.com/oauth2/token
---
