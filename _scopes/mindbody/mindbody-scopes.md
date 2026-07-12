---
authorization_urls:
- https://signin.mindbodyonline.com/connect/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Mindbody Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mindbody publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mindbody API on a user''s behalf.


  Tokens are issued from https://signin.mindbodyonline.com/connect/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mindbody
provider_slug: mindbody
schemes:
- description: OpenID Connect bearer token issued by Mindbody Identity Service (signin.mindbodyonline.com). Required for endpoints that act on behalf of a staff or client user.
  flows:
  - authorizationUrl: https://signin.mindbodyonline.com/connect/authorize
    flow: authorizationCode
    tokenUrl: https://signin.mindbodyonline.com/connect/token
  name: OAuth2
  source: openapi/mindbody-public-api-v6-openapi-original.yml
scope_count: 5
scope_names:
- Mindbody.Api.Public.v6
- email
- offline_access
- openid
- profile
scopes:
- description: Access the Mindbody Public API v6 on behalf of the user.
  flows:
  - authorizationCode
  scope: Mindbody.Api.Public.v6
- description: User email claim.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token.
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect base scope.
  flows:
  - authorizationCode
  scope: openid
- description: User profile claims.
  flows:
  - authorizationCode
  scope: profile
slug: mindbody-scopes
source_filename: mindbody-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mindbody-public-api-v6-openapi-original.yml\nschemes:\n- name: OAuth2\n  source: openapi/mindbody-public-api-v6-openapi-original.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://signin.mindbodyonline.com/connect/authorize\n    tokenUrl: https://signin.mindbodyonline.com/connect/token\n  description: OpenID Connect bearer token issued by Mindbody Identity Service (signin.mindbodyonline.com).\n    Required for endpoints that act on behalf of a staff or client user.\nscopes:\n- scope: Mindbody.Api.Public.v6\n  description: Access the Mindbody Public API v6 on behalf of the user.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mindbody-public-api-v6-openapi-original.yml\n- scope: email\n  description: User email claim.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mindbody-public-api-v6-openapi-original.yml\n- scope: offline_access\n  description: Issue a refresh token.\n  flows:\n\
  \  - authorizationCode\n  sources:\n  - openapi/mindbody-public-api-v6-openapi-original.yml\n- scope: openid\n  description: OpenID Connect base scope.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mindbody-public-api-v6-openapi-original.yml\n- scope: profile\n  description: User profile claims.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/mindbody-public-api-v6-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mindbody/refs/heads/main/scopes/mindbody-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Fitness
- Wellness
- Beauty
- Scheduling
- Booking
- Point of Sale
- Studios
- Salons
- Spas
- Webhooks
token_urls:
- https://signin.mindbodyonline.com/connect/token
---
