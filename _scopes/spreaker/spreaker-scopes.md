---
authorization_urls:
- https://www.spreaker.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Spreaker Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Spreaker publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Spreaker API on a user''s behalf.


  Tokens are issued from https://api.spreaker.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Spreaker
provider_slug: spreaker
schemes:
- description: OAuth2. Authorize at https://www.spreaker.com/oauth2/authorize and exchange or refresh tokens at https://api.spreaker.com/oauth2/token. Access tokens are sent as a Bearer token in the Authorization header.
  flows:
  - authorizationUrl: https://www.spreaker.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://api.spreaker.com/oauth2/token
  name: oauth2
  source: openapi/spreaker-openapi.yml
scope_count: 1
scope_names:
- basic
scopes:
- description: Basic access to the Spreaker API on behalf of the user.
  flows:
  - authorizationCode
  scope: basic
slug: spreaker-scopes
source_filename: spreaker-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spreaker-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/spreaker-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.spreaker.com/oauth2/authorize\n    tokenUrl: https://api.spreaker.com/oauth2/token\n  description: OAuth2. Authorize at https://www.spreaker.com/oauth2/authorize and exchange or\n    refresh tokens at https://api.spreaker.com/oauth2/token. Access tokens are sent as a Bearer\n    token in the Authorization header.\nscopes:\n- scope: basic\n  description: Basic access to the Spreaker API on behalf of the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/spreaker-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spreaker/refs/heads/main/scopes/spreaker-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Podcasting
- Podcast Hosting
- Audio
- Media
- Monetization
- Analytics
token_urls:
- https://api.spreaker.com/oauth2/token
---
