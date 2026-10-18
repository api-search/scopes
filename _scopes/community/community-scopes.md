---
api_specs:
- filename: community-member-data-api-openapi.yml
  format: yaml
  label: Community Member Data API
  slug: community-member-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-member-data-api-openapi.yml
- filename: community-messaging-api-openapi.yml
  format: yaml
  label: Community Messaging API
  slug: community-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-messaging-api-openapi.yml
- filename: community-tags-api-openapi.yml
  format: yaml
  label: Community Tags API
  slug: community-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/openapi/community-tags-api-openapi.yml
authorization_urls:
- https://oauth-login.community.com/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: none
name: Community Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Community uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /oauth/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Community
provider_slug: community
schemes:
- flows:
  - authorizationUrl: https://oauth-login.community.com/
    flow: authorizationCode
    tokenUrl: /oauth/v1/token
  name: oAuth
  source: openapi/community-member-data-api-openapi.yml
- flows:
  - authorizationUrl: https://oauth-login.community.com/
    flow: authorizationCode
    tokenUrl: /oauth/v1/token
  name: oAuth
  source: openapi/community-messaging-api-openapi.yml
- flows:
  - authorizationUrl: https://oauth-login.community.com/
    flow: authorizationCode
    tokenUrl: /oauth/v1/token
  name: oAuth
  source: openapi/community-tags-api-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: community-scopes
source_filename: community-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/community-member-data-api-openapi.yml, openapi/community-messaging-api-openapi.yml,\n  openapi/community-tags-api-openapi.yml\nschemes:\n- name: oAuth\n  source: openapi/community-member-data-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth-login.community.com/\n    tokenUrl: /oauth/v1/token\n- name: oAuth\n  source: openapi/community-messaging-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth-login.community.com/\n    tokenUrl: /oauth/v1/token\n- name: oAuth\n  source: openapi/community-tags-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://oauth-login.community.com/\n    tokenUrl: /oauth/v1/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/community/refs/heads/main/scopes/community-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Messaging
- SMS
- Communications
- Marketing
- Creators
- Webhook
- Company
token_bound: false
token_urls:
- /oauth/v1/token
---
