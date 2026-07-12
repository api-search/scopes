---
authorization_urls: []
description: ''
docs: https://bandcamp.com/developer
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Bandcamp Scopes
name_suffix: OAuth Scopes
note: Bandcamp's API uses the OAuth 2.0 client_credentials grant (with refresh tokens) and does not define or document any OAuth scopes (https://bandcamp.com/developer).
overview: 'Bandcamp uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://bandcamp.com/oauth_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bandcamp
provider_slug: bandcamp
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://bandcamp.com/oauth_token
  name: oauth2
  source: openapi/bandcamp-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: bandcamp-scopes
source_filename: bandcamp-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bandcamp-openapi.yml\ndocs: https://bandcamp.com/developer\nnote: Bandcamp's API uses the OAuth 2.0 client_credentials grant (with refresh tokens)\n  and does not define or document any OAuth scopes (https://bandcamp.com/developer).\nschemes:\n- name: oauth2\n  source: openapi/bandcamp-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://bandcamp.com/oauth_token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bandcamp/refs/heads/main/scopes/bandcamp-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Music
- Marketplace
- Indie
- Audio
- Sales
- Merch
token_urls:
- https://bandcamp.com/oauth_token
---
