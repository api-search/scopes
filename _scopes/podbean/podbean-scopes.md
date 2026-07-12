---
authorization_urls:
- https://api.podbean.com/v1/dialog/oauth
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Podbean Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Podbean publishes 3 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Podbean API on a user''s behalf.


  Tokens are issued from https://api.podbean.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Podbean
provider_slug: podbean
schemes:
- description: OAuth 2.0. Register an app at developers.podbean.com to obtain a Client ID and Secret.
  flows:
  - authorizationUrl: https://api.podbean.com/v1/dialog/oauth
    flow: authorizationCode
    tokenUrl: https://api.podbean.com/v1/oauth/token
  - flow: clientCredentials
    tokenUrl: https://api.podbean.com/v1/oauth/token
  name: oauth2
  source: openapi/podbean-openapi.yml
scope_count: 3
scope_names:
- episode_publish
- episode_read
- podcast_read
scopes:
- description: Publish and manage episodes.
  flows:
  - authorizationCode
  - clientCredentials
  scope: episode_publish
- description: Read episodes.
  flows:
  - authorizationCode
  scope: episode_read
- description: Read podcast profile and settings.
  flows:
  - authorizationCode
  - clientCredentials
  scope: podcast_read
slug: podbean-scopes
source_filename: podbean-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/podbean-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/podbean-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.podbean.com/v1/dialog/oauth\n    tokenUrl: https://api.podbean.com/v1/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://api.podbean.com/v1/oauth/token\n  description: OAuth 2.0. Register an app at developers.podbean.com to obtain a Client ID and\n    Secret.\nscopes:\n- scope: episode_publish\n  description: Publish and manage episodes.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/podbean-openapi.yml\n- scope: episode_read\n  description: Read episodes.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/podbean-openapi.yml\n- scope: podcast_read\n  description: Read podcast profile and settings.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - openapi/podbean-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/podbean/refs/heads/main/scopes/podbean-scopes.yml
summary_line: 3 scopes · authorizationCode/clientCredentials
tags:
- Podcasting
- Podcast Hosting
- Media
- Audio
- Episodes
- Analytics
- Monetization
token_urls:
- https://api.podbean.com/v1/oauth/token
---
