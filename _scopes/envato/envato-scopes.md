---
authorization_urls:
- https://api.envato.com/authorization
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Envato Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Envato publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Envato API on a user''s behalf.


  Tokens are issued from https://api.envato.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Envato
provider_slug: envato
schemes:
- flows:
  - authorizationUrl: https://api.envato.com/authorization
    flow: authorizationCode
    tokenUrl: https://api.envato.com/token
  name: oauth2
  source: openapi/envato-openapi.yml
scope_count: 1
scope_names:
- default
scopes:
- description: Default Envato Market scope set
  flows:
  - authorizationCode
  scope: default
slug: envato-scopes
source_filename: envato-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/envato-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/envato-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.envato.com/authorization\n    tokenUrl: https://api.envato.com/token\nscopes:\n- scope: default\n  description: Default Envato Market scope set\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/envato-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envato/refs/heads/main/scopes/envato-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Stock Media
- Marketplace
- Themes
- Audio
- Video
- Graphics
- Subscription
token_urls:
- https://api.envato.com/token
---
