---
authorization_urls: []
description: 'OAuth surface of the HKEX FINI API Gateway. FINI does not use a classic named-scope catalog: the OAuth 2.0 JWT-bearer token response returns the participant''s Company ID as the scope value (e.g. "scope": "CP00001"), and endpoint-level authorization is instead governed by ForgeRock entitlement functions assigned to the participant''s profile on the HKEX Access Management Portal. The three entitlement functions below are the effective permission groups for the API''s three endpoint categories.'
docs: https://www.hkex.com.hk/Services/Platform-Services/FINI?sc_lang=en
flows:
- urn:ietf:params:oauth:grant-type:jwt-bearer
kind: oauth-scopes
layout: scope
method: searched
name: Hkex Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'HKEX uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://openam.connect.hkex.com.hk/openam/oauth2/eu/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HKEX
provider_slug: hkex
schemes:
- flows:
  - flow: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://openam.connect.hkex.com.hk/openam/oauth2/eu/access_token
  name: FINI OAuth 2.0 JWT-bearer
scope_count: 0
scope_names: []
scopes: []
slug: hkex-scopes
source_filename: hkex-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-22'\nmethod: searched\nsource: https://www.hkex.com.hk/-/media/HKEX-Market/Services/Next-Generation-Post-Trade-Programme/Fini/FINI-API-User-Guide-v0,-d-,41.pdf\ndocs: https://www.hkex.com.hk/Services/Platform-Services/FINI?sc_lang=en\ndescription: >-\n  OAuth surface of the HKEX FINI API Gateway. FINI does not use a classic\n  named-scope catalog: the OAuth 2.0 JWT-bearer token response returns the\n  participant's Company ID as the scope value (e.g. \"scope\": \"CP00001\"), and\n  endpoint-level authorization is instead governed by ForgeRock entitlement\n  functions assigned to the participant's profile on the HKEX Access\n  Management Portal. The three entitlement functions below are the effective\n  permission groups for the API's three endpoint categories.\nschemes:\n- name: FINI OAuth 2.0 JWT-bearer\n  flows:\n  - flow: 'urn:ietf:params:oauth:grant-type:jwt-bearer'\n    tokenUrl: https://openam.connect.hkex.com.hk/openam/oauth2/eu/access_token\nscope_model:\
  \ >-\n  Token \"scope\" carries the Company ID rather than permissions; permissions are\n  ForgeRock functions bound to the registered Agent/Machine profiles.\npermissions:\n- permission: EU_finiIPORefDataAPI\n  grants: /api/ipos/*\n  description: Enquire IPO list and IPO reference data — available to all FINI user categories.\n- permission: EU_finiPOSubAPI\n  grants: /api/eipo/subscriptions/*\n  description: Add, change, invalidate and enquire EIPO public-offer subscription entries — HKSCC Participants.\n- permission: EU_finiPOFundAPI\n  grants: /api/eipo/funding/*\n  description: Confirm and enquire EIPO funding statuses — EIPO Designated Banks.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hkex/refs/heads/main/scopes/hkex-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Financial
- Market Data
- Stocks
- Derivatives
- Exchange
- Real-Time
- Historical Data
- Order Book
- Reference Data
- IPO
token_urls:
- https://openam.connect.hkex.com.hk/openam/oauth2/eu/access_token
---
