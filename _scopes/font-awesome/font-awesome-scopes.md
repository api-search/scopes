---
authorization_urls: []
description: ''
docs: https://docs.fontawesome.com/apis/graphql/auth
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Font Awesome Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Font Awesome publishes 8 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Font Awesome API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Font Awesome
provider_slug: font-awesome
schemes: []
scope_count: 8
scope_names:
- public
- kits_read
- kits_download
- profile_read
- domains_read
- entitlements_read
- svg_icons_free
- svg_icons_pro
scopes:
- description: Default scope granted to all requests, including unauthenticated ones; access to free/public metadata.
  flows: []
  scope: public
- description: Read-only access to Kit configuration metadata and the account's icon uploads (Pro).
  flows: []
  scope: kits_read
- description: Permits downloading Kits (Pro).
  flows: []
  scope: kits_download
- description: Read-only access to personally identifiable account information such as email address.
  flows: []
  scope: profile_read
- description: Read-only access to the account's CDN referrer/domain whitelist (Pro).
  flows: []
  scope: domains_read
- description: Read-only access to account entitlements — the features/Icon Collections the account may use.
  flows: []
  scope: entitlements_read
- description: Read-only access to SVG path data for Font Awesome Free icons.
  flows: []
  scope: svg_icons_free
- description: Read-only access to SVG path data for Pro-exclusive families plus all Free SVGs (Pro).
  flows: []
  scope: svg_icons_pro
slug: font-awesome-scopes
source_filename: font-awesome-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fontawesome.com/apis/graphql/auth\ndocs: https://docs.fontawesome.com/apis/graphql/auth\nmodel: >-\n  Scopes are attached to an account API token; the access token minted at the\n  token endpoint inherits those scopes. Account holders can self-generate tokens\n  with the `public` and `kits_read` scopes; other scopes require contacting\n  Font Awesome support.\ntoken_endpoint: https://api.fontawesome.com/token\nscopes:\n  - scope: public\n    description: Default scope granted to all requests, including unauthenticated ones; access to free/public metadata.\n    self_serviceable: true\n  - scope: kits_read\n    description: Read-only access to Kit configuration metadata and the account's icon uploads (Pro).\n    self_serviceable: true\n  - scope: kits_download\n    description: Permits downloading Kits (Pro).\n    self_serviceable: false\n  - scope: profile_read\n    description: Read-only access to personally identifiable\
  \ account information such as email address.\n    self_serviceable: false\n  - scope: domains_read\n    description: Read-only access to the account's CDN referrer/domain whitelist (Pro).\n    self_serviceable: false\n  - scope: entitlements_read\n    description: Read-only access to account entitlements — the features/Icon Collections the account may use.\n    self_serviceable: false\n  - scope: svg_icons_free\n    description: Read-only access to SVG path data for Font Awesome Free icons.\n    self_serviceable: false\n  - scope: svg_icons_pro\n    description: Read-only access to SVG path data for Pro-exclusive families plus all Free SVGs (Pro).\n    self_serviceable: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/font-awesome/refs/heads/main/scopes/font-awesome-scopes.yml
summary_line: 8 scopes
tags:
- Icons
- SVG
- Fonts
- Web Design
- Developer Tools
- GraphQL
- Icon Library
- Frontend
- Design System
- Company
token_urls: []
---
