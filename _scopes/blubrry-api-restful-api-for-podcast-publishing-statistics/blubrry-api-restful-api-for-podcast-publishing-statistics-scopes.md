---
authorization_urls:
- https://api.blubrry.com/oauth2/authorize
description: ''
docs: https://blubrry.com/developer/api/oauth-2/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Blubrry Api Restful Api For Podcast Publishing Statistics Scopes
name_suffix: OAuth Scopes
note: Blubrry's OAuth 2.0 implementation does not use or document scopes — the token response returns "scope":null and access is granted at the level of the account authorized during the authorization code flow (https://blubrry.com/developer/api/oauth-2/).
overview: 'Blubrry API uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.blubrry.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blubrry API
provider_slug: blubrry-api-restful-api-for-podcast-publishing-statistics
schemes:
- description: 'OAuth 2.0 Bearer token. Contact Blubrry to receive a client_id and

    secret. Tokens expire after one hour; refresh tokens do not expire.'
  flows:
  - authorizationUrl: https://api.blubrry.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.blubrry.com/oauth2/token
  name: OAuth2
  source: openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: blubrry-api-restful-api-for-podcast-publishing-statistics-scopes
source_filename: blubrry-api-restful-api-for-podcast-publishing-statistics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-openapi.yml\ndocs: https://blubrry.com/developer/api/oauth-2/\nnote: Blubrry's OAuth 2.0 implementation does not use or document scopes — the token\n  response returns \"scope\":null and access is granted at the level of the account\n  authorized during the authorization code flow (https://blubrry.com/developer/api/oauth-2/).\nschemes:\n- name: OAuth2\n  source: openapi/blubrry-api-restful-api-for-podcast-publishing-statistics-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.blubrry.com/oauth2/authorize\n    tokenUrl: https://api.blubrry.com/oauth2/token\n  description: |-\n    OAuth 2.0 Bearer token. Contact Blubrry to receive a client_id and\n    secret. Tokens expire after one hour; refresh tokens do not expire.\nscopes: []\n"
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
