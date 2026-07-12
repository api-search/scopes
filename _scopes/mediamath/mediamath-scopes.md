---
authorization_urls:
- https://auth.mediamath.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Mediamath Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'MediaMath publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the MediaMath API on a user''s behalf.


  Tokens are issued from https://auth.mediamath.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: MediaMath
provider_slug: mediamath
schemes:
- flows:
  - authorizationUrl: https://auth.mediamath.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.mediamath.com/oauth/token
  name: Auth0
  source: openapi/campaigns-api-openapi.yaml
- flows:
  - authorizationUrl: https://auth.mediamath.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.mediamath.com/oauth/token
  name: Auth0
  source: openapi/reporting-api-openapi.yaml
scope_count: 2
scope_names:
- manage:services
- offline_access
scopes:
- description: normal access
  flows:
  - authorizationCode
  scope: manage:services
- description: for refresh tokens
  flows:
  - authorizationCode
  scope: offline_access
slug: mediamath-scopes
source_filename: mediamath-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/campaigns-api-openapi.yaml, openapi/reporting-api-openapi.yaml\nschemes:\n- name: Auth0\n  source: openapi/campaigns-api-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mediamath.com/authorize\n    tokenUrl: https://auth.mediamath.com/oauth/token\n- name: Auth0\n  source: openapi/reporting-api-openapi.yaml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.mediamath.com/authorize\n    tokenUrl: https://auth.mediamath.com/oauth/token\nscopes:\n- scope: manage:services\n  description: normal access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/campaigns-api-openapi.yaml\n- scope: offline_access\n  description: for refresh tokens\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/campaigns-api-openapi.yaml\n  - openapi/reporting-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediamath/refs/heads/main/scopes/mediamath-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Programmatic Advertising
- DSP
- Demand-Side Platform
- Campaign Management
- Ad Tech
- Bidding
- Audience Segments
- Creative Management
- Reporting
- Analytics
token_urls:
- https://auth.mediamath.com/oauth/token
---
