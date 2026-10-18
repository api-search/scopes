---
api_specs:
- filename: anilist-oauth2-api-openapi.yml
  format: yaml
  label: AniList O Auth2 API
  slug: anilist-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anilist/refs/heads/main/openapi/anilist-oauth2-api-openapi.yml
- filename: anilist-graph-ql-api-openapi.yml
  format: yaml
  label: AniList Graph QL API
  slug: anilist-graph-ql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anilist/refs/heads/main/openapi/anilist-graph-ql-api-openapi.yml
authorization_urls:
- https://anilist.co/api/v2/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: none
name: Anilist Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'AniList uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://anilist.co/api/v2/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AniList
provider_slug: anilist
schemes:
- description: AniList OAuth2 (no scopes supported)
  flows:
  - authorizationUrl: https://anilist.co/api/v2/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://anilist.co/api/v2/oauth/token
  - authorizationUrl: https://anilist.co/api/v2/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/anilist-graph-ql-api-openapi.yml
- description: AniList OAuth2 (no scopes supported)
  flows:
  - authorizationUrl: https://anilist.co/api/v2/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://anilist.co/api/v2/oauth/token
  - authorizationUrl: https://anilist.co/api/v2/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/anilist-oauth2-api-openapi.yml
- description: AniList OAuth2 (no scopes supported)
  flows:
  - authorizationUrl: https://anilist.co/api/v2/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://anilist.co/api/v2/oauth/token
  - authorizationUrl: https://anilist.co/api/v2/oauth/authorize
    flow: implicit
  name: oauth2
  source: openapi/anilist-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: anilist-scopes
source_filename: anilist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: none\nsource: openapi/anilist-graph-ql-api-openapi.yml, openapi/anilist-oauth2-api-openapi.yml, openapi/anilist-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/anilist-graph-ql-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n    tokenUrl: https://anilist.co/api/v2/oauth/token\n  - flow: implicit\n    authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n  description: AniList OAuth2 (no scopes supported)\n- name: oauth2\n  source: openapi/anilist-oauth2-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n    tokenUrl: https://anilist.co/api/v2/oauth/token\n  - flow: implicit\n    authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n  description: AniList OAuth2 (no scopes supported)\n- name: oauth2\n  source: openapi/anilist-openapi.yml\n  flows:\n  - flow: authorizationCode\n \
  \   authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n    tokenUrl: https://anilist.co/api/v2/oauth/token\n  - flow: implicit\n    authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n  description: AniList OAuth2 (no scopes supported)\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anilist/refs/heads/main/scopes/anilist-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Anime
- Manga
- Entertainment
- Media
- Social
- Database
- GraphQL
- Authentication
- Public APIs
token_bound: false
token_urls:
- https://anilist.co/api/v2/oauth/token
---
