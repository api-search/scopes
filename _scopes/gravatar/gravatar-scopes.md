---
authorization_urls:
- https://public-api.wordpress.com/oauth2/authorize
description: ''
docs: https://docs.gravatar.com/api/oauth/
flows:
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Gravatar Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gravatar publishes 3 OAuth 2.0 scopes via the implicit flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gravatar API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gravatar
provider_slug: gravatar
schemes:
- description: WordPress OAuth token to authenticate the request.
  flows:
  - authorizationUrl: https://public-api.wordpress.com/oauth2/authorize
    flow: implicit
  name: oauth
  source: openapi/openapi.json
scope_count: 3
scope_names:
- auth
- gravatar-profile:read
- gravatar-profile:manage
scopes:
- description: Required to work with any Gravatar endpoints; allows the user to authenticate.
  flows: []
  scope: auth
- description: Allows access to the user's profile information, like avatar, about info, or display name.
  flows: []
  scope: gravatar-profile:read
- description: Allows editing the user's profile information, like avatar, about info, or display name.
  flows: []
  scope: gravatar-profile:manage
slug: gravatar-scopes
source_filename: gravatar-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/openapi.json\ndocs: https://docs.gravatar.com/api/oauth/\nschemes:\n- name: oauth\n  source: openapi/openapi.json\n  flows:\n  - flow: implicit\n    authorizationUrl: https://public-api.wordpress.com/oauth2/authorize\n  description: WordPress OAuth token to authenticate the request.\nscopes:\n- scope: auth\n  description: Required to work with any Gravatar endpoints; allows the user to authenticate.\n  sources:\n  - https://docs.gravatar.com/api/oauth/\n- scope: gravatar-profile:read\n  description: Allows access to the user's profile information, like avatar, about\n    info, or display name.\n  sources:\n  - https://docs.gravatar.com/api/oauth/\n- scope: gravatar-profile:manage\n  description: Allows editing the user's profile information, like avatar, about\n    info, or display name.\n  sources:\n  - https://docs.gravatar.com/api/oauth/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gravatar/refs/heads/main/scopes/gravatar-scopes.yml
summary_line: 3 scopes · implicit
tags:
- Avatars
- Identity
- Profiles
- Social
- Images
- GraphQL
- REST
token_urls: []
---
