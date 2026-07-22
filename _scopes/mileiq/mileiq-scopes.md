---
api_specs:
- filename: mileiq-external-openapi-original.json
  format: json
  label: MileIQ External API
  slug: mileiq-external-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mileiq/refs/heads/main/openapi/mileiq-external-openapi-original.json
authorization_urls:
- https://oauth2.mileiq.com/oauth2/auth
description: ''
docs: https://developer.mileiq.com/api-reference/getting-started
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Mileiq Scopes
name_suffix: OAuth Scopes
note: The OpenAPI does not declare oauth2 flows or scopes; scopes are documented in the developer portal (the getting-started OAuth example requests "drives:read:all users:read") and enforced via 403 responses whose descriptions name the required scope. The authorization server advertises the OIDC baseline scopes (openid, offline, offline_access).
overview: 'MileIQ publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MileIQ API on a user''s behalf.


  Tokens are issued from https://oauth2.mileiq.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MileIQ
provider_slug: mileiq
schemes:
- flows:
  - authorizationUrl: https://oauth2.mileiq.com/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.mileiq.com/oauth2/token
  name: OAuth2
  source: https://developer.mileiq.com/api-reference/getting-started
scope_count: 7
scope_names:
- users:read
- drives:read:all
- groups:read
- groups:read:reported-drives
- openid
- offline_access
- offline
scopes:
- description: Read access to user profile information.
  flows: []
  scope: users:read
- description: Read access to a user's drive (mileage trip) records.
  flows: []
  scope: drives:read:all
- description: Read access to groups (teams) the authenticated user administers.
  flows: []
  scope: groups:read
- description: Read access to drives reported to a group for review.
  flows: []
  scope: groups:read:reported-drives
- description: OIDC authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Issue a refresh token for offline access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Legacy alias for offline_access advertised by the authorization server.
  flows: []
  scope: offline
slug: mileiq-scopes
source_filename: mileiq-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developer.mileiq.com/api-reference/getting-started.md\ndocs: https://developer.mileiq.com/api-reference/getting-started\noidc_discovery: https://oauth2.mileiq.com/.well-known/openid-configuration\nnote: >-\n  The OpenAPI does not declare oauth2 flows or scopes; scopes are documented in the\n  developer portal (the getting-started OAuth example requests \"drives:read:all users:read\")\n  and enforced via 403 responses whose descriptions name the required scope. The\n  authorization server advertises the OIDC baseline scopes (openid, offline, offline_access).\nschemes:\n  - name: OAuth2\n    source: https://developer.mileiq.com/api-reference/getting-started\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://oauth2.mileiq.com/oauth2/auth\n        tokenUrl: https://oauth2.mileiq.com/oauth2/token\nscopes:\n  - scope: users:read\n    description: Read access to user profile information.\n    internal_name:\
  \ users_read\n    operations: [get_me, get_user]\n    sources: [https://developer.mileiq.com/api-reference/getting-started]\n  - scope: drives:read:all\n    description: Read access to a user's drive (mileage trip) records.\n    operations: [get_user_drives]\n    sources: [https://developer.mileiq.com/api-reference/getting-started]\n  - scope: groups:read\n    description: Read access to groups (teams) the authenticated user administers.\n    internal_name: groups_read\n    operations: [get_groups, get_group]\n    sources: [openapi/mileiq-external-openapi-original.json]\n  - scope: groups:read:reported-drives\n    description: Read access to drives reported to a group for review.\n    internal_name: groups_read_reported_drives\n    operations: [get_group_reported_drives]\n    sources: [openapi/mileiq-external-openapi-original.json]\n  - scope: openid\n    description: OIDC authentication; issue an ID token.\n    flows: [authorizationCode]\n    sources: [https://oauth2.mileiq.com/.well-known/openid-configuration]\n\
  \  - scope: offline_access\n    description: Issue a refresh token for offline access.\n    flows: [authorizationCode]\n    sources: [https://oauth2.mileiq.com/.well-known/openid-configuration]\n  - scope: offline\n    description: Legacy alias for offline_access advertised by the authorization server.\n    sources: [https://oauth2.mileiq.com/.well-known/openid-configuration]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mileiq/refs/heads/main/scopes/mileiq-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Consumer
- Mileage Tracking
- Expense Management
- Transportation
- Tax
- Accounting
- Location
- Fleet
token_urls:
- https://oauth2.mileiq.com/oauth2/token
---
