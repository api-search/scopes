---
authorization_urls: []
description: ''
docs: https://www.ti.com/developer-api/store-api/authentication.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Texas Instruments Scopes
name_suffix: OAuth Scopes
note: TI APIs use the OAuth 2.0 client credentials flow with no published scopes — the token response returns an empty scope field and access is granted per API via myTI API key requests (https://www.ti.com/developer-api/store-api/authentication.html).
overview: 'Texas Instruments uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://transact.ti.com/v1/oauth/accesstoken.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Texas Instruments
provider_slug: texas-instruments
schemes:
- description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret from your myTI developer account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken
  name: OAuth2
  source: openapi/texas-instruments-product-information-openapi.yml
- description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret from your myTI company account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken
  name: OAuth2
  source: openapi/texas-instruments-store-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: texas-instruments-scopes
source_filename: texas-instruments-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/texas-instruments-product-information-openapi.yml, openapi/texas-instruments-store-openapi.yml\ndocs: https://www.ti.com/developer-api/store-api/authentication.html\nnote: TI APIs use the OAuth 2.0 client credentials flow with no published scopes — the\n  token response returns an empty scope field and access is granted per API via myTI\n  API key requests (https://www.ti.com/developer-api/store-api/authentication.html).\nschemes:\n- name: OAuth2\n  source: openapi/texas-instruments-product-information-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken\n  description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret\n    from your myTI developer account.\n- name: OAuth2\n  source: openapi/texas-instruments-store-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://transact.ti.com/v1/oauth/accesstoken\n\
  \  description: OAuth 2.0 client credentials flow. Obtain access token using client_id and client_secret\n    from your myTI company account.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/texas-instruments/refs/heads/main/scopes/texas-instruments-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Electronics
- Ordering
- Semiconductors
- Supply Chain
- Fortune 500
token_urls:
- https://transact.ti.com/v1/oauth/accesstoken
---
