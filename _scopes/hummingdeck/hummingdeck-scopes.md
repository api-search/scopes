---
api_specs:
- filename: hummingdeck-companies-api-openapi.yml
  format: yaml
  label: HummingDeck Companies API
  slug: hummingdeck-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-companies-api-openapi.yml
- filename: hummingdeck-contacts-api-openapi.yml
  format: yaml
  label: HummingDeck Contacts API
  slug: hummingdeck-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-contacts-api-openapi.yml
- filename: hummingdeck-decisions-api-openapi.yml
  format: yaml
  label: HummingDeck Decisions API
  slug: hummingdeck-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-decisions-api-openapi.yml
- filename: hummingdeck-decks-api-openapi.yml
  format: yaml
  label: HummingDeck Decks API
  slug: hummingdeck-decks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-decks-api-openapi.yml
- filename: hummingdeck-emails-api-openapi.yml
  format: yaml
  label: HummingDeck Emails API
  slug: hummingdeck-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-emails-api-openapi.yml
- filename: hummingdeck-hooks-api-openapi.yml
  format: yaml
  label: HummingDeck Hooks API
  slug: hummingdeck-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-hooks-api-openapi.yml
- filename: hummingdeck-me-api-openapi.yml
  format: yaml
  label: HummingDeck Me API
  slug: hummingdeck-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-me-api-openapi.yml
- filename: hummingdeck-room-labels-api-openapi.yml
  format: yaml
  label: HummingDeck Room Labels API
  slug: hummingdeck-room-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-room-labels-api-openapi.yml
- filename: hummingdeck-room-views-api-openapi.yml
  format: yaml
  label: HummingDeck Room Views API
  slug: hummingdeck-room-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-room-views-api-openapi.yml
- filename: hummingdeck-rooms-api-openapi.yml
  format: yaml
  label: HummingDeck Rooms API
  slug: hummingdeck-rooms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-rooms-api-openapi.yml
- filename: hummingdeck-shares-api-openapi.yml
  format: yaml
  label: HummingDeck Shares API
  slug: hummingdeck-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-shares-api-openapi.yml
- filename: hummingdeck-views-api-openapi.yml
  format: yaml
  label: HummingDeck Views API
  slug: hummingdeck-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/openapi/hummingdeck-views-api-openapi.yml
authorization_urls:
- https://app.hummingdeck.com/api/zapier/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Hummingdeck Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'HummingDeck uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://app.hummingdeck.com/api/zapier/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: HummingDeck
provider_slug: hummingdeck
schemes:
- description: Issued by the Zapier integration's OAuth flow. Access tokens last 30 days; refresh tokens last 90 days. The only credential accepted on webhook subscription endpoints.
  flows:
  - authorizationUrl: https://app.hummingdeck.com/api/zapier/authorize
    flow: authorizationCode
    tokenUrl: https://app.hummingdeck.com/api/zapier/token
  name: oauth2
  source: openapi/hummingdeck-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: hummingdeck-scopes
source_filename: hummingdeck-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: none\nsource: openapi/hummingdeck-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/hummingdeck-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.hummingdeck.com/api/zapier/authorize\n    tokenUrl: https://app.hummingdeck.com/api/zapier/token\n  description: Issued by the Zapier integration's OAuth flow. Access tokens last 30 days; refresh\n    tokens last 90 days. The only credential accepted on webhook subscription endpoints.\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hummingdeck/refs/heads/main/scopes/hummingdeck-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Document Sharing
- Engagement Analytics
- Digital Sales Rooms
- Data Rooms
- Client Portals
- Integrations
- Secure Sharing
token_bound: false
token_urls:
- https://app.hummingdeck.com/api/zapier/token
---
