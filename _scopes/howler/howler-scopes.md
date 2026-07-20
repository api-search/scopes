---
api_specs:
- filename: howler-consumer-portal-openapi.yml
  format: yaml
  label: Howler API v3 (Consumer Portal)
  slug: howler-api-v3-consumer-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-consumer-portal-openapi.yml
- filename: howler-webhooks-openapi.yml
  format: yaml
  label: Howler Webhooks v1
  slug: howler-webhooks-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-webhooks-openapi.yml
authorization_urls:
- /oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Howler Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Howler publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Howler API on a user''s behalf.


  Tokens are issued from /oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Howler
provider_slug: howler
schemes:
- description: OAuth2 authentication for third-party applications
  flows:
  - authorizationUrl: /oauth/authorize
    flow: authorizationCode
    tokenUrl: /oauth/token
  name: oauth2
  source: openapi/howler-consumer-portal-openapi.yml
scope_count: 3
scope_names:
- login
- ott
- public
scopes:
- description: Login scope
  flows:
  - authorizationCode
  scope: login
- description: One-time token scope
  flows:
  - authorizationCode
  scope: ott
- description: Public scope
  flows:
  - authorizationCode
  scope: public
slug: howler-scopes
source_filename: howler-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/howler-consumer-portal-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/howler-consumer-portal-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth/authorize\n    tokenUrl: /oauth/token\n  description: OAuth2 authentication for third-party applications\nscopes:\n- scope: login\n  description: Login scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/howler-consumer-portal-openapi.yml\n- scope: ott\n  description: One-time token scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/howler-consumer-portal-openapi.yml\n- scope: public\n  description: Public scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/howler-consumer-portal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/scopes/howler-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- Events
- Ticketing
- Payments
- Cashless
- RFID
- Event Management
- Fintech
- South Africa
token_urls:
- /oauth/token
---
