---
authorization_urls: []
description: ''
docs: https://github.com/moodysanalytics/databuffet-api-codesamples/blob/master/dataBuffet-api-userguide.md
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Moodys Scopes
name_suffix: OAuth Scopes
note: Moody's APIs do not use OAuth scopes — the Data Buffet API user guide (https://github.com/moodysanalytics/databuffet-api-codesamples/blob/master/dataBuffet-api-userguide.md) documents an OAuth2 client_credentials flow with access/encryption keys and no scope parameter, and permissions across Moody's products are tied to account entitlements and roles rather than scopes.
overview: 'Moody''s uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.economy.com/data/v1/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Moody's
provider_slug: moodys
schemes:
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-data-buffet-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: moodys-scopes
source_filename: moodys-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moodys-data-buffet-api-openapi.yml\ndocs: https://github.com/moodysanalytics/databuffet-api-codesamples/blob/master/dataBuffet-api-userguide.md\nnote: Moody's APIs do not use OAuth scopes — the Data Buffet API user guide (https://github.com/moodysanalytics/databuffet-api-codesamples/blob/master/dataBuffet-api-userguide.md)\n  documents an OAuth2 client_credentials flow with access/encryption keys and no scope\n  parameter, and permissions across Moody's products are tied to account entitlements\n  and roles rather than scopes.\nschemes:\n- name: oauth2\n  source: openapi/moodys-data-buffet-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys/refs/heads/main/scopes/moodys-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Climate Risk
- Compliance
- Credit Risk
- Economic Data
- Entity Verification
- Financial Analytics
- Insurance
- KYC
- Risk
- Screening
token_urls:
- https://api.economy.com/data/v1/oauth2/token
---
