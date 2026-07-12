---
authorization_urls:
- https://discogs.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Discogs Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Discogs publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Discogs API on a user''s behalf.


  Tokens are issued from https://api.discogs.com/oauth/access_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Discogs
provider_slug: discogs
schemes:
- description: OAuth 1.0a flow modeled as OAuth2 for tooling. Required for write actions on behalf of other users.
  flows:
  - authorizationUrl: https://discogs.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.discogs.com/oauth/access_token
  name: OAuth1
  source: openapi/discogs-openapi-original.yml
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read user data
  flows:
  - authorizationCode
  scope: read
- description: Write/update user resources
  flows:
  - authorizationCode
  scope: write
slug: discogs-scopes
source_filename: discogs-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/discogs-openapi-original.yml\nschemes:\n- name: OAuth1\n  source: openapi/discogs-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://discogs.com/oauth/authorize\n    tokenUrl: https://api.discogs.com/oauth/access_token\n  description: OAuth 1.0a flow modeled as OAuth2 for tooling. Required for write actions on\n    behalf of other users.\nscopes:\n- scope: read\n  description: Read user data\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/discogs-openapi-original.yml\n- scope: write\n  description: Write/update user resources\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/discogs-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/discogs/refs/heads/main/scopes/discogs-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Music
- Marketplace
- Catalog
- Community
- Vinyl
- Public APIs
token_urls:
- https://api.discogs.com/oauth/access_token
---
