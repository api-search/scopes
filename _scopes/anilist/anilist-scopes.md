---
api_specs:
- filename: anilist-openapi.yml
  format: yaml
  label: AniList GraphQL API v2
  slug: anilist-graphql-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anilist/refs/heads/main/openapi/anilist-openapi.yml
authorization_urls:
- https://anilist.co/api/v2/oauth/authorize
description: ''
docs: https://docs.anilist.co/guide/auth/
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: derived
name: Anilist Scopes
name_suffix: OAuth Scopes
note: AniList's OAuth2 does not use scopes — the auth docs state "Scopes are not supported. Access tokens provide (almost) full access to a user's data" (https://docs.anilist.co/guide/auth/).
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
  source: openapi/anilist-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: anilist-scopes
source_filename: anilist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anilist-openapi.yml\ndocs: https://docs.anilist.co/guide/auth/\nnote: AniList's OAuth2 does not use scopes — the auth docs state \"Scopes are not\n  supported. Access tokens provide (almost) full access to a user's data\"\n  (https://docs.anilist.co/guide/auth/).\nschemes:\n- name: oauth2\n  source: openapi/anilist-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n    tokenUrl: https://anilist.co/api/v2/oauth/token\n  - flow: implicit\n    authorizationUrl: https://anilist.co/api/v2/oauth/authorize\n  description: AniList OAuth2 (no scopes supported)\nscopes: []\n"
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
- OAuth2
- Public APIs
token_urls:
- https://anilist.co/api/v2/oauth/token
---
