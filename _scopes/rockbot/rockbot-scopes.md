---
api_specs:
- filename: rockbot-audio-messaging-api-openapi.yml
  format: yaml
  label: Rockbot Audio Messaging API
  slug: rockbot-audio-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-audio-messaging-api-openapi.yml
- filename: rockbot-auth-api-openapi.yml
  format: yaml
  label: Rockbot Auth API
  slug: rockbot-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-auth-api-openapi.yml
- filename: rockbot-data-api-openapi.yml
  format: yaml
  label: Rockbot Data API
  slug: rockbot-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-data-api-openapi.yml
- filename: rockbot-devices-api-openapi.yml
  format: yaml
  label: Rockbot Devices API
  slug: rockbot-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-devices-api-openapi.yml
- filename: rockbot-music-api-openapi.yml
  format: yaml
  label: Rockbot Music API
  slug: rockbot-music-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-music-api-openapi.yml
- filename: rockbot-signage-api-openapi.yml
  format: yaml
  label: Rockbot Signage API
  slug: rockbot-signage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/openapi/rockbot-signage-api-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.rockbot.com/start.html
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Rockbot Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Rockbot uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rockbot
provider_slug: rockbot
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: rockbot-scopes
source_filename: rockbot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.rockbot.com/start.html\ndocs: https://developer.rockbot.com/start.html\nscope_count: 3\nnotes: >-\n  UPGRADED from derived to searched. Rockbot's REST API DOES have a scope model —\n  the Getting Started page states plainly: \"Your credentials only grant access to\n  the scopes you requested.\" Scopes are therefore bound to the API client at\n  issuance time and negotiated by email, not requested per-token. But Rockbot\n  publishes NO scope reference, NO permission matrix, and NO scope names, and the\n  OpenAPI's oauth2 flow declares an empty scopes object. So the scope surface is\n  real and undiscoverable at the same time: an integrator cannot know what to ask\n  for without asking a human. The only enumerable scopes anywhere in the Rockbot\n  estate belong to the SEPARATE MCP authorization server, and they are the three\n  generic OIDC scopes listed below — not Rockbot resource scopes.\nrest_api:\n  scopes_documented:\
  \ false\n  scopes_enumerable: false\n  model: >-\n    Per-client, granted at credential issuance based on \"which features you'd\n    like to access via the Rockbot API\" (quoted from the access-request\n    instructions). Effective scope is whatever Rockbot support approved.\n  request_process: >-\n    Email support@rockbot.com, subject \"Rockbot API Access Request\", naming the\n    features required.\n  scopes: []\n  scopes_note: >-\n    Empty because Rockbot names none — an honest gap, not an assertion that the\n    API is unscoped. openapi/rockbot-auth-api-openapi.yml declares the\n    clientCredentials flow with zero scopes for the same reason.\n  inferable_capability_groups:\n    note: >-\n      NOT SCOPES. Listed only as the feature axes a requester would name in the\n      access-request email, taken from the API's own tag structure.\n    groups: [Music, Audio Messaging, Signage, Devices, Data]\nmcp_server:\n  issuer: https://auth.rockbot.com/application/o/mcp-server/\n  source:\
  \ https://auth.rockbot.com/application/o/mcp-server/.well-known/openid-configuration\n  saved: well-known/rockbot-mcp-authorization-server.json\n  scopes_documented: true\n  scopes:\n    - name: openid\n      description: Standard OIDC scope — request an ID token.\n      standard: true\n    - name: email\n      description: Standard OIDC scope — release the email claim.\n      standard: true\n    - name: profile\n      description: >-\n        Standard OIDC scope — release profile claims (name, given_name,\n        preferred_username, nickname, groups).\n      standard: true\n  scopes_note: >-\n    All three are generic OpenID Connect scopes emitted by the authentik default\n    provider. NO Rockbot-specific resource scope (music, signage, devices, data)\n    is advertised in discovery, so what a Rockbot MCP token is actually\n    authorized to do cannot be determined from the published metadata.\nclaims_supported:\n  - sub\n  - iss\n  - aud\n  - exp\n  - iat\n  - auth_time\n  - acr\n\
  \  - amr\n  - nonce\n  - email\n  - email_verified\n  - name\n  - given_name\n  - preferred_username\n  - nickname\n  - groups\n"
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
token_urls: []
---
