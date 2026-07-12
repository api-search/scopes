---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Navan Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Navan publishes 6 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Navan API on a user''s behalf.


  Tokens are issued from https://app.navan.com/ta-auth/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Navan
provider_slug: navan
schemes:
- description: 'OAuth 2.0 client-credentials flow. Generate a client_id / client_secret in the Navan app under Settings > Integrations (API), then POST grant_type=client_credentials to the token URL to obtain a Bearer access token. US token URL: https://app.navan.com/ta-auth/oauth/token ; EU token URL: https://app-fra.navan.com/ta-auth/oauth/token . (Some integrations reference an https://api.navan.com/ta-auth/oauth/token or /auth/v1/token variant; confirm the current token URL in the Navan developer portal.)'
  flows:
  - flow: clientCredentials
    tokenUrl: https://app.navan.com/ta-auth/oauth/token
  name: oauth2ClientCredentials
  source: openapi/navan-openapi.yml
scope_count: 6
scope_names:
- bookings:read
- liquid:read
- liquid:write
- users:delete
- users:read
- users:write
scopes:
- description: Read booking (trip) data.
  flows:
  - clientCredentials
  scope: bookings:read
- description: Read expense data (transactions, fees, receipts, custom fields).
  flows:
  - clientCredentials
  scope: liquid:read
- description: Update expense data.
  flows:
  - clientCredentials
  scope: liquid:write
- description: Deactivate users.
  flows:
  - clientCredentials
  scope: users:delete
- description: Read user profiles.
  flows:
  - clientCredentials
  scope: users:read
- description: Create and modify users.
  flows:
  - clientCredentials
  scope: users:write
slug: navan-scopes
source_filename: navan-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/navan-openapi.yml\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/navan-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://app.navan.com/ta-auth/oauth/token\n  description: 'OAuth 2.0 client-credentials flow. Generate a client_id / client_secret in the\n    Navan app under Settings > Integrations (API), then POST grant_type=client_credentials to\n    the token URL to obtain a Bearer access token. US token URL: https://app.navan.com/ta-auth/oauth/token\n    ; EU token URL: https://app-fra.navan.com/ta-auth/oauth/token . (Some integrations reference\n    an https://api.navan.com/ta-auth/oauth/token or /auth/v1/token variant; confirm the current\n    token URL in the Navan developer portal.)'\nscopes:\n- scope: bookings:read\n  description: Read booking (trip) data.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/navan-openapi.yml\n- scope: liquid:read\n  description: Read\
  \ expense data (transactions, fees, receipts, custom fields).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/navan-openapi.yml\n- scope: liquid:write\n  description: Update expense data.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/navan-openapi.yml\n- scope: users:delete\n  description: Deactivate users.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/navan-openapi.yml\n- scope: users:read\n  description: Read user profiles.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/navan-openapi.yml\n- scope: users:write\n  description: Create and modify users.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/navan-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navan/refs/heads/main/scopes/navan-scopes.yml
summary_line: 6 scopes · clientCredentials
tags:
- Corporate Travel
- Expense Management
- Corporate Cards
- Spend Management
- T&E
- Fintech
- Business Travel
token_urls:
- https://app.navan.com/ta-auth/oauth/token
---
