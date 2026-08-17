---
api_specs:
- filename: snapchat-ads-api-openapi.yml
  format: yaml
  label: Snapchat Ads API
  slug: snapchat-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ads-api-openapi.yml
- filename: snapchat-ad-accounts-api-openapi.yml
  format: yaml
  label: Snapchat Ad Accounts API
  slug: snapchat-ad-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ad-accounts-api-openapi.yml
- filename: snapchat-ad-squads-api-openapi.yml
  format: yaml
  label: Snapchat Ad Squads API
  slug: snapchat-ad-squads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-ad-squads-api-openapi.yml
- filename: snapchat-audience-segments-api-openapi.yml
  format: yaml
  label: Snapchat Audience Segments API
  slug: snapchat-audience-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-audience-segments-api-openapi.yml
- filename: snapchat-campaigns-api-openapi.yml
  format: yaml
  label: Snapchat Campaigns API
  slug: snapchat-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-campaigns-api-openapi.yml
- filename: snapchat-conversion-events-api-openapi.yml
  format: yaml
  label: Snapchat Conversion Events API
  slug: snapchat-conversion-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-conversion-events-api-openapi.yml
- filename: snapchat-creatives-api-openapi.yml
  format: yaml
  label: Snapchat Creatives API
  slug: snapchat-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-creatives-api-openapi.yml
- filename: snapchat-funding-sources-api-openapi.yml
  format: yaml
  label: Snapchat Funding Sources API
  slug: snapchat-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-funding-sources-api-openapi.yml
- filename: snapchat-measurement-api-openapi.yml
  format: yaml
  label: Snapchat Measurement API
  slug: snapchat-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-measurement-api-openapi.yml
- filename: snapchat-media-api-openapi.yml
  format: yaml
  label: Snapchat Media API
  slug: snapchat-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-media-api-openapi.yml
- filename: snapchat-oauth-api-openapi.yml
  format: yaml
  label: Snapchat OAuth API
  slug: snapchat-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-oauth-api-openapi.yml
- filename: snapchat-organizations-api-openapi.yml
  format: yaml
  label: Snapchat Organizations API
  slug: snapchat-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-organizations-api-openapi.yml
- filename: snapchat-user-profile-api-openapi.yml
  format: yaml
  label: Snapchat User Profile API
  slug: snapchat-user-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/openapi/snapchat-user-profile-api-openapi.yml
authorization_urls: []
description: 'Snap''s OAuth scope surface is deliberately narrow and splits across three authorization servers. Login Kit publishes four fully-qualified URI scopes covering identity only — Snap states plainly that Login Kit "does not provide access to personal user data, such as private messages, shared content or contacts". The Marketing API is coarse: one scope for the whole ads surface, with real authorization carried by Business Manager ROLES rather than scopes. The Ads MCP server has exactly one scope, snapads.read, matching its read-only release.'
docs: https://developers.snap.com/snap-kit/login-kit/overview#scopes
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Snapchat Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Snapchat publishes 7 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Snapchat API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Snapchat
provider_slug: snapchat
schemes:
- authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth
  flows:
  - authorizationCode
  - implicit
  name: loginKitOAuth
  pkce: S256
  source: https://developers.snap.com/snap-kit/login-kit/overview
  tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token
- authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth
  flows:
  - authorizationCode
  name: bearerAuth
  source: openapi/snapchat-ads-api-openapi.yml
  tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token
- authorizationUrl: https://mcp.snapchat.com/authorize
  flows:
  - authorizationCode
  name: mcpOAuth
  pkce: S256
  source: https://mcp.snapchat.com/.well-known/oauth-authorization-server/ads
  tokenUrl: https://mcp.snapchat.com/token
scope_count: 7
scope_names:
- https://auth.snapchat.com/oauth2/api/user.display_name
- https://auth.snapchat.com/oauth2/api/user.external_id
- https://auth.snapchat.com/oauth2/api/user.bitmoji.avatar
- https://auth.snapchat.com/oauth2/api/camkit_lens_push_to_device
- https://auth.snapchat.com/oauth2/api/user
- snapads.read
- snapchat-marketing-api
scopes:
- description: Grants access to the user's display name.
  flows:
  - authorizationCode
  - implicit
  scope: https://auth.snapchat.com/oauth2/api/user.display_name
- description: Grants access to a unique app-specific user ID. Pseudonymous and scoped per application — the same Snapchatter has a different external_id in every integrating app.
  flows:
  - authorizationCode
  - implicit
  scope: https://auth.snapchat.com/oauth2/api/user.external_id
- description: Grants access to the user's Bitmoji avatar.
  flows:
  - authorizationCode
  - implicit
  scope: https://auth.snapchat.com/oauth2/api/user.bitmoji.avatar
- description: Enables Lens Push-to-Device for Camera Kit-enabled apps. Automatically available to apps with Camera Kit enabled and cannot be toggled by users.
  flows: []
  scope: https://auth.snapchat.com/oauth2/api/camkit_lens_push_to_device
- description: 'Parent scope value observed in Snap''s own documented token-endpoint response examples (`"scope": "https://auth.snapchat.com/oauth2/api/user"`). Not listed in the scope table; it appears to be the granted-scope form returned after exchange rather than a scope to request.'
  flows: []
  scope: https://auth.snapchat.com/oauth2/api/user
- description: Read-only access to authorized Snapchat Ads data through https://mcp.snapchat.com/ads. The only scope the MCP authorization server accepts — Snap's own docs warn that omitting it causes the bridge to request a default set the server rejects.
  flows:
  - authorizationCode
  scope: snapads.read
- description: Single coarse scope covering the entire Marketing API surface — organizations, ad accounts, campaigns, ad squads, ads, creatives, media, audience segments, funding sources and measurement. There is no read/write split and no per-resource scope.
  flows:
  - authorizationCode
  scope: snapchat-marketing-api
slug: snapchat-scopes
source_filename: snapchat-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://developers.snap.com/snap-kit/login-kit/overview#scopes,\n  https://developers.snap.com/marketing-api/Ads-MCP/Introduction,\n  https://mcp.snapchat.com/.well-known/oauth-authorization-server/ads, openapi/*.yml\ndocs: https://developers.snap.com/snap-kit/login-kit/overview#scopes\nprovider: Snapchat\nproviderId: snapchat\ndescription: >-\n  Snap's OAuth scope surface is deliberately narrow and splits across three authorization servers.\n  Login Kit publishes four fully-qualified URI scopes covering identity only — Snap states plainly\n  that Login Kit \"does not provide access to personal user data, such as private messages, shared\n  content or contacts\". The Marketing API is coarse: one scope for the whole ads surface, with real\n  authorization carried by Business Manager ROLES rather than scopes. The Ads MCP server has\n  exactly one scope, snapads.read, matching its read-only release.\nschemes:\n- name: loginKitOAuth\n\
  \  authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth\n  tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token\n  flows:\n  - authorizationCode\n  - implicit\n  pkce: S256\n  source: https://developers.snap.com/snap-kit/login-kit/overview\n- name: bearerAuth\n  authorizationUrl: https://accounts.snapchat.com/accounts/oauth2/auth\n  tokenUrl: https://accounts.snapchat.com/login/oauth2/access_token\n  flows:\n  - authorizationCode\n  source: openapi/snapchat-ads-api-openapi.yml\n- name: mcpOAuth\n  authorizationUrl: https://mcp.snapchat.com/authorize\n  tokenUrl: https://mcp.snapchat.com/token\n  flows:\n  - authorizationCode\n  pkce: S256\n  source: https://mcp.snapchat.com/.well-known/oauth-authorization-server/ads\nscopes:\n- scope: https://auth.snapchat.com/oauth2/api/user.display_name\n  product: Login Kit\n  description: Grants access to the user's display name.\n  user_toggleable: false\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - https://developers.snap.com/snap-kit/login-kit/overview\n\
  - scope: https://auth.snapchat.com/oauth2/api/user.external_id\n  product: Login Kit\n  description: >-\n    Grants access to a unique app-specific user ID. Pseudonymous and scoped per application — the\n    same Snapchatter has a different external_id in every integrating app.\n  user_toggleable: false\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - https://developers.snap.com/snap-kit/login-kit/overview\n- scope: https://auth.snapchat.com/oauth2/api/user.bitmoji.avatar\n  product: Login Kit\n  description: Grants access to the user's Bitmoji avatar.\n  user_toggleable: true\n  flows:\n  - authorizationCode\n  - implicit\n  sources:\n  - https://developers.snap.com/snap-kit/login-kit/overview\n- scope: https://auth.snapchat.com/oauth2/api/camkit_lens_push_to_device\n  product: Camera Kit\n  description: >-\n    Enables Lens Push-to-Device for Camera Kit-enabled apps. Automatically available to apps with\n    Camera Kit enabled and cannot be toggled by users.\n  user_toggleable:\
  \ false\n  conditional: Available only to applications with Camera Kit enabled.\n  sources:\n  - https://developers.snap.com/snap-kit/login-kit/overview\n- scope: https://auth.snapchat.com/oauth2/api/user\n  product: Login Kit\n  description: >-\n    Parent scope value observed in Snap's own documented token-endpoint response examples\n    (`\"scope\": \"https://auth.snapchat.com/oauth2/api/user\"`). Not listed in the scope table; it\n    appears to be the granted-scope form returned after exchange rather than a scope to request.\n  user_toggleable: null\n  note: Recorded because it appears verbatim in the docs, flagged because the docs do not define it.\n  sources:\n  - https://developers.snap.com/snap-kit/login-kit/overview\n- scope: snapads.read\n  product: Snapchat Ads MCP Server\n  description: >-\n    Read-only access to authorized Snapchat Ads data through https://mcp.snapchat.com/ads. The only\n    scope the MCP authorization server accepts — Snap's own docs warn that omitting\
  \ it causes the\n    bridge to request a default set the server rejects.\n  flows:\n  - authorizationCode\n  sources:\n  - https://developers.snap.com/marketing-api/Ads-MCP/connect-an-agent\n- scope: snapchat-marketing-api\n  product: Snapchat Marketing API\n  description: >-\n    Single coarse scope covering the entire Marketing API surface — organizations, ad accounts,\n    campaigns, ad squads, ads, creatives, media, audience segments, funding sources and\n    measurement. There is no read/write split and no per-resource scope.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/snapchat-ads-api-openapi.yml\nscope_count: 7\nauthorization_model_note: >-\n  Scopes are not where Marketing API authorization actually lives. Snap states \"the access token\n  reflects the user's permissions, so API calls are scoped to what that user can access\" — the\n  effective permission set comes from Business Manager roles (admin, member, and since 2026-07-01\n  agency_admin and agency_member),\
  \ not from the OAuth scope string. A least-privilege review of a\n  Snap integration has to look at roles, not at the scopes requested.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snapchat/refs/heads/main/scopes/snapchat-scopes.yml
summary_line: 7 scopes · authorizationCode/implicit
tags:
- Advertising
- AR
- Augmented Reality
- Marketing
- Messaging
- Social Media
token_urls: []
---
