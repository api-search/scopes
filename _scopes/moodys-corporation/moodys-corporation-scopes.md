---
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Moodys Corporation Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Moody''s Corporation publishes 2 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Moody''s Corporation API on a user''s behalf.


  Tokens are issued from https://api.economy.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Moody's Corporation
provider_slug: moodys-corporation
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/oauth2/token
  name: oauth2
  source: openapi/moodys-analytics-developer-openapi.yml
- description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id and client_secret from your Moody's Analytics account.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.economy.com/data/v1/oauth2/token
  name: oauth2
  source: openapi/moodys-data-buffet-api-openapi.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to entitled Moody's Analytics products
  flows:
  - clientCredentials
  scope: read
- description: Write access for job submission and basket / order management
  flows:
  - clientCredentials
  scope: write
slug: moodys-corporation-scopes
source_filename: moodys-corporation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moodys-analytics-developer-openapi.yml, openapi/moodys-data-buffet-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/moodys-analytics-developer-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/oauth2/token\n- name: oauth2\n  source: openapi/moodys-data-buffet-api-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.economy.com/data/v1/oauth2/token\n  description: OAuth2 client credentials flow for authenticating API requests. Obtain client_id\n    and client_secret from your Moody's Analytics account.\nscopes:\n- scope: read\n  description: Read access to entitled Moody's Analytics products\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moodys-analytics-developer-openapi.yml\n- scope: write\n  description: Write access for job submission and basket / order management\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/moodys-analytics-developer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moodys-corporation/refs/heads/main/scopes/moodys-corporation-scopes.yml
summary_line: 2 scopes · clientCredentials
tags:
- Analytics
- Catastrophe Risk
- Climate Risk
- Compliance
- Credit Ratings
- Economic Data
- ESG
- Financial Data
- KYC
- Risk
- Fortune 1000
token_urls:
- https://api.economy.com/oauth2/token
- https://api.economy.com/data/v1/oauth2/token
---
