---
api_specs:
- filename: soundcloud-openapi.yml
  format: yaml
  label: SoundCloud API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soundcloud/refs/heads/main/openapi/soundcloud-openapi.yml
authorization_urls:
- https://secure.soundcloud.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Soundcloud Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SoundCloud publishes 1 OAuth 2.0 scope via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the SoundCloud API on a user''s behalf.


  Tokens are issued from https://secure.soundcloud.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SoundCloud
provider_slug: soundcloud
schemes:
- description: 'OAuth 2.1 with PKCE. Access tokens are short-lived (~1 hour). Use

    Authorization: OAuth {ACCESS_TOKEN} on each request.'
  flows:
  - authorizationUrl: https://secure.soundcloud.com/authorize
    flow: authorizationCode
    tokenUrl: https://secure.soundcloud.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://secure.soundcloud.com/oauth/token
  name: oauth2
  source: openapi/soundcloud-openapi.yml
scope_count: 1
scope_names:
- non-expiring
scopes:
- description: Non-expiring refresh-token grant
  flows:
  - authorizationCode
  scope: non-expiring
slug: soundcloud-scopes
source_filename: soundcloud-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/soundcloud-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/soundcloud-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.soundcloud.com/authorize\n    tokenUrl: https://secure.soundcloud.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://secure.soundcloud.com/oauth/token\n  description: |-\n    OAuth 2.1 with PKCE. Access tokens are short-lived (~1 hour). Use\n    Authorization: OAuth {ACCESS_TOKEN} on each request.\nscopes:\n- scope: non-expiring\n  description: Non-expiring refresh-token grant\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/soundcloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundcloud/refs/heads/main/scopes/soundcloud-scopes.yml
summary_line: 1 scope · authorizationCode/clientCredentials
tags:
- Music
- Streaming
- Audio
- OAuth
- Tracks
- Playlists
token_urls:
- https://secure.soundcloud.com/oauth/token
---
