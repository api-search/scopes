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
overview: 'Rockbot publishes 3 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Rockbot API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Rockbot
provider_slug: rockbot
schemes: []
scope_count: 3
scope_names:
- openid
- email
- profile
scopes:
- description: Standard OIDC scope — request an ID token.
  flows: []
  scope: openid
- description: Standard OIDC scope — release the email claim.
  flows: []
  scope: email
- description: Standard OIDC scope — release profile claims (name, given_name, preferred_username, nickname, groups).
  flows: []
  scope: profile
slug: rockbot-scopes
source_filename: rockbot-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.rockbot.com/start.html\ndocs: https://developer.rockbot.com/start.html\nscope_count: 3\nnotes: 'UPGRADED from derived to searched. Rockbot''s REST API DOES have a scope model\n  — the Getting Started page states plainly: \"Your credentials only grant access to\n  the scopes you requested.\" Scopes are therefore bound to the API client at issuance\n  time and negotiated by email, not requested per-token. But Rockbot publishes NO\n  scope reference, NO permission matrix, and NO scope names, and the OpenAPI''s oauth2\n  flow declares an empty scopes object. So the scope surface is real and undiscoverable\n  at the same time: an integrator cannot know what to ask for without asking a human.\n  The only enumerable scopes anywhere in the Rockbot estate belong to the SEPARATE\n  MCP authorization server, and they are the three generic OIDC scopes listed below\n  — not Rockbot resource scopes.'\nrest_api:\n  scopes_documented:\
  \ false\n  scopes_enumerable: false\n  model: Per-client, granted at credential issuance based on \"which features you'd\n    like to access via the Rockbot API\" (quoted from the access-request instructions).\n    Effective scope is whatever Rockbot support approved.\n  request_process: Email support@rockbot.com, subject \"Rockbot API Access Request\",\n    naming the features required.\n  scopes: []\n  scopes_note: Empty because Rockbot names none — an honest gap, not an assertion\n    that the API is unscoped. openapi/rockbot-auth-api-openapi.yml declares the clientCredentials\n    flow with zero scopes for the same reason.\n  inferable_capability_groups:\n    note: NOT SCOPES. Listed only as the feature axes a requester would name in the\n      access-request email, taken from the API's own tag structure.\n    groups:\n    - Music\n    - Audio Messaging\n    - Signage\n    - Devices\n    - Data\nmcp_server:\n  issuer: https://auth.rockbot.com/application/o/mcp-server/\n  source: https://auth.rockbot.com/application/o/mcp-server/.well-known/openid-configuration\n\
  \  saved: well-known/rockbot-mcp-authorization-server.json\n  scopes_documented: true\n  scopes: &id001\n  - name: openid\n    description: Standard OIDC scope — request an ID token.\n    standard: true\n  - name: email\n    description: Standard OIDC scope — release the email claim.\n    standard: true\n  - name: profile\n    description: Standard OIDC scope — release profile claims (name, given_name, preferred_username,\n      nickname, groups).\n    standard: true\n  scopes_note: All three are generic OpenID Connect scopes emitted by the authentik\n    default provider. NO Rockbot-specific resource scope (music, signage, devices,\n    data) is advertised in discovery, so what a Rockbot MCP token is actually authorized\n    to do cannot be determined from the published metadata.\nclaims_supported:\n- sub\n- iss\n- aud\n- exp\n- iat\n- auth_time\n- acr\n- amr\n- nonce\n- email\n- email_verified\n- name\n- given_name\n- preferred_username\n- nickname\n- groups\nscopes: *id001\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rockbot/refs/heads/main/scopes/rockbot-scopes.yml
summary_line: 3 scopes
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
token_bound: false
token_urls: []
---
