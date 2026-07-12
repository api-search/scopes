---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Formance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Formance publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Formance API on a user''s behalf.


  Tokens are issued from https://{organization}.{environment}.formance.cloud/api/auth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Formance
provider_slug: formance
schemes:
- description: 'OAuth2 client-credentials flow. Exchange a client id and secret at `/api/auth/oauth/token` for a Bearer access token, then send it as `Authorization: Bearer <token>`.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://{organization}.{environment}.formance.cloud/api/auth/oauth/token
  name: oauth2
  source: openapi/formance-openapi.yml
scope_count: 6
scope_names:
- ledger:read
- ledger:write
- payments:read
- payments:write
- wallets:read
- wallets:write
scopes:
- description: Read ledger resources
  flows:
  - clientCredentials
  scope: ledger:read
- description: Write ledger resources
  flows:
  - clientCredentials
  scope: ledger:write
- description: Read payments resources
  flows:
  - clientCredentials
  scope: payments:read
- description: Write payments resources
  flows:
  - clientCredentials
  scope: payments:write
- description: Read wallets resources
  flows:
  - clientCredentials
  scope: wallets:read
- description: Write wallets resources
  flows:
  - clientCredentials
  scope: wallets:write
slug: formance-scopes
source_filename: formance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formance-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/formance-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{organization}.{environment}.formance.cloud/api/auth/oauth/token\n  description: 'OAuth2 client-credentials flow. Exchange a client id and secret at `/api/auth/oauth/token`\n    for a Bearer access token, then send it as `Authorization: Bearer <token>`.'\nscopes:\n- scope: ledger:read\n  description: Read ledger resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/formance-openapi.yml\n- scope: ledger:write\n  description: Write ledger resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/formance-openapi.yml\n- scope: payments:read\n  description: Read payments resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/formance-openapi.yml\n- scope: payments:write\n  description: Write payments resources\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/formance-openapi.yml\n- scope: wallets:read\n  description: Read wallets resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/formance-openapi.yml\n- scope: wallets:write\n  description: Write wallets resources\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/formance-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formance/refs/heads/main/scopes/formance-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Financial Infrastructure
- Ledger
- Double-Entry Accounting
- Payments
- Orchestration
- Money Movement
- Open Source
- Fintech
token_urls:
- https://{organization}.{environment}.formance.cloud/api/auth/oauth/token
---
