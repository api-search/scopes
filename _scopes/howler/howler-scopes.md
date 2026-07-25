---
api_specs:
- filename: howler-artists-api-openapi.yml
  format: yaml
  label: Howler Artists API
  slug: howler-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-artists-api-openapi.yml
- filename: howler-assign-ticket-api-openapi.yml
  format: yaml
  label: Howler Assign Ticket API
  slug: howler-assign-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-assign-ticket-api-openapi.yml
- filename: howler-bank-account-api-openapi.yml
  format: yaml
  label: Howler Bank Account API
  slug: howler-bank-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-bank-account-api-openapi.yml
- filename: howler-basic-authentication-api-openapi.yml
  format: yaml
  label: Howler Basic Authentication API
  slug: howler-basic-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-basic-authentication-api-openapi.yml
- filename: howler-cashless-tags-api-openapi.yml
  format: yaml
  label: Howler Cashless Tags API
  slug: howler-cashless-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-cashless-tags-api-openapi.yml
- filename: howler-cashout-api-openapi.yml
  format: yaml
  label: Howler Cashout API
  slug: howler-cashout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-cashout-api-openapi.yml
- filename: howler-email-otp-api-openapi.yml
  format: yaml
  label: Howler Email OTP API
  slug: howler-email-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-email-otp-api-openapi.yml
- filename: howler-events-api-openapi.yml
  format: yaml
  label: Howler Events API
  slug: howler-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-events-api-openapi.yml
- filename: howler-oauth-api-openapi.yml
  format: yaml
  label: Howler OAuth API
  slug: howler-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-oauth-api-openapi.yml
- filename: howler-third-party-oauth-api-openapi.yml
  format: yaml
  label: Howler Third Party OAuth API
  slug: howler-third-party-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-third-party-oauth-api-openapi.yml
- filename: howler-tickets-api-openapi.yml
  format: yaml
  label: Howler Tickets API
  slug: howler-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-tickets-api-openapi.yml
- filename: howler-top-up-api-openapi.yml
  format: yaml
  label: Howler Top Up API
  slug: howler-top-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-top-up-api-openapi.yml
- filename: howler-top-up-cashless-tag-api-openapi.yml
  format: yaml
  label: Howler Top Up Cashless Tag API
  slug: howler-top-up-cashless-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-top-up-cashless-tag-api-openapi.yml
- filename: howler-top-up-ticket-api-openapi.yml
  format: yaml
  label: Howler Top Up Ticket API
  slug: howler-top-up-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-top-up-ticket-api-openapi.yml
- filename: howler-topupables-api-openapi.yml
  format: yaml
  label: Howler Topupables API
  slug: howler-topupables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-topupables-api-openapi.yml
- filename: howler-transfer-ticket-api-openapi.yml
  format: yaml
  label: Howler Transfer Ticket API
  slug: howler-transfer-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-transfer-ticket-api-openapi.yml
- filename: howler-user-api-openapi.yml
  format: yaml
  label: Howler User API
  slug: howler-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-user-api-openapi.yml
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
