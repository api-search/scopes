---
api_specs:
- filename: blubrry-api-restful-api-for-podcast-publishing-statistics-episode-api-openapi.yml
  format: yaml
  label: Blubrry API Episode API
  slug: blubrry-api-restful-api-for-podcast-publishing-statistics-episode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-episode-api-openapi.yml
- filename: blubrry-api-restful-api-for-podcast-publishing-statistics-media-api-openapi.yml
  format: yaml
  label: Blubrry API Media API
  slug: blubrry-api-restful-api-for-podcast-publishing-statistics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-media-api-openapi.yml
- filename: blubrry-api-restful-api-for-podcast-publishing-statistics-statistics-api-openapi.yml
  format: yaml
  label: Blubrry API Statistics API
  slug: blubrry-api-restful-api-for-podcast-publishing-statistics-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-statistics-api-openapi.yml
- filename: blubrry-api-restful-api-for-podcast-publishing-statistics-podcaster-openapi.yaml
  format: yaml
  label: Blubrry Podcast Hosting & Statistics API (v2)
  slug: blubrry-podcast-hosting-statistics-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-podcaster-openapi.yaml
authorization_urls:
- https://api.blubrry.com/oauth2/authorize
description: ''
docs: https://blubrry.com/developer/api/oauth-2/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Blubrry Api Restful Api For Podcast Publishing Statistics Scopes
name_suffix: OAuth Scopes
note: 'Blubrry''s OAuth 2.0 implementation does not use or document scopes. The published token response on https://blubrry.com/developer/api/oauth-2/ returns "scope": null, and access is granted at the level of the whole Blubrry account authorized during the authorization-code flow. There is no scope reference page and the OpenAPI declares no oauth2 scopes. An honest zero, not a gap in our search.'
overview: 'Blubrry API uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.blubrry.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blubrry API
provider_slug: blubrry-api-restful-api-for-podcast-publishing-statistics
schemes:
- description: 'OAuth 2.0 Bearer token, account-wide. Tokens expire after one hour; refresh tokens do

    not expire. No scope parameter is accepted or returned.'
  flows:
  - authorizationUrl: https://api.blubrry.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.blubrry.com/oauth2/token
  name: OAuth2
  source: https://blubrry.com/developer/api/oauth-2/
scope_count: 0
scope_names: []
scopes: []
slug: blubrry-api-restful-api-for-podcast-publishing-statistics-scopes
source_filename: blubrry-api-restful-api-for-podcast-publishing-statistics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://blubrry.com/developer/api/oauth-2/\ndocs: https://blubrry.com/developer/api/oauth-2/\nnote: >-\n  Blubrry's OAuth 2.0 implementation does not use or document scopes. The published token\n  response on https://blubrry.com/developer/api/oauth-2/ returns \"scope\": null, and access is\n  granted at the level of the whole Blubrry account authorized during the authorization-code\n  flow. There is no scope reference page and the OpenAPI declares no oauth2 scopes. An honest\n  zero, not a gap in our search.\nscope_count: 0\nscopes_supported: false\nschemes:\n- name: OAuth2\n  source: https://blubrry.com/developer/api/oauth-2/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.blubrry.com/oauth2/authorize\n    tokenUrl: https://api.blubrry.com/oauth2/token\n  description: |-\n    OAuth 2.0 Bearer token, account-wide. Tokens expire after one hour; refresh tokens do\n    not expire. No scope parameter is\
  \ accepted or returned.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blubrry-api-restful-api-for-podcast-publishing-statistics/refs/heads/main/scopes/blubrry-api-restful-api-for-podcast-publishing-statistics-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Podcasting
- Audio
- Media
- Publishing
- Statistics
token_urls:
- https://api.blubrry.com/oauth2/token
---
