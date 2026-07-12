---
authorization_urls:
- https://sketchfab.com/oauth2/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Sketchfab Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Sketchfab publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sketchfab API on a user''s behalf.


  Tokens are issued from https://sketchfab.com/oauth2/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sketchfab
provider_slug: sketchfab
schemes:
- flows:
  - authorizationUrl: https://sketchfab.com/oauth2/authorize/
    flow: authorizationCode
    tokenUrl: https://sketchfab.com/oauth2/token/
  name: OAuth2
  source: openapi/sketchfab-download-api-openapi.yml
scope_count: 1
scope_names:
- read
scopes:
- description: Read access including model downloads.
  flows:
  - authorizationCode
  scope: read
slug: sketchfab-scopes
source_filename: sketchfab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sketchfab-download-api-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/sketchfab-download-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sketchfab.com/oauth2/authorize/\n    tokenUrl: https://sketchfab.com/oauth2/token/\nscopes:\n- scope: read\n  description: Read access including model downloads.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/sketchfab-download-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sketchfab/refs/heads/main/scopes/sketchfab-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- 3D
- Models
- Marketplace
- Viewer
- WebGL
- glTF
- AR
- VR
- Creative
- Epic Games
token_urls:
- https://sketchfab.com/oauth2/token/
---
