---
api_specs:
- filename: rockbot-openapi.yml
  format: yaml
  label: Rockbot API
  slug: rockbot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Rockbot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rockbot uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.rockbot.com/v5/api-clients/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rockbot
provider_slug: rockbot
schemes:
- description: 'OAuth 2.0 Client Credentials grant. Exchange a CLIENT_ID/CLIENT_SECRET (issued by Rockbot support) at the token endpoint for a 24-hour bearer ACCESS_TOKEN, then send it as `Authorization: Bearer ACCESS_TOKEN`.'
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.rockbot.com/v5/api-clients/token
  name: oauth2
  source: openapi/rockbot-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: rockbot-scopes
source_filename: rockbot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/rockbot-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/rockbot-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.rockbot.com/v5/api-clients/token\n  description: 'OAuth 2.0 Client Credentials grant. Exchange a CLIENT_ID/CLIENT_SECRET (issued\n    by Rockbot support) at the token endpoint for a 24-hour bearer ACCESS_TOKEN, then send it\n    as `Authorization: Bearer ACCESS_TOKEN`.'\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/scopes/rockbot-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer
- Music
- Digital Signage
- Audio Messaging
- Retail Media
- In-Location Media
- Media
- Entertainment
token_urls:
- https://api.rockbot.com/v5/api-clients/token
---
