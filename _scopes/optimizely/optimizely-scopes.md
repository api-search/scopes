---
authorization_urls: []
description: ''
docs: https://docs.developers.optimizely.com/web-experimentation/docs/registration
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Optimizely Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Optimizely publishes 4 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Optimizely API on a user''s behalf.


  Tokens are issued from https://api.cmp.optimizely.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Optimizely
provider_slug: optimizely
schemes:
- description: OAuth 2.0 authentication for the CMP API.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.cmp.optimizely.com/oauth/token
  name: oauth2
  source: openapi/optimizely-cmp-openapi.yml
scope_count: 4
scope_names:
- all
- openid
- profile
- offline_access
scopes:
- description: The only supported scope for the Optimizely Web Experimentation REST API OAuth 2.0 flow. The generated token has permissions that match the user role of the authorizing user.
  flows: []
  scope: all
- description: OpenID Connect scope used in the Optimizely CMP authorization code flow to identify the user.
  flows: []
  scope: openid
- description: OpenID Connect scope used in the Optimizely CMP authorization code flow to access user profile information.
  flows: []
  scope: profile
- description: OpenID Connect scope used in the Optimizely CMP authorization code flow to obtain refresh tokens for long-lived access.
  flows: []
  scope: offline_access
slug: optimizely-scopes
source_filename: optimizely-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: searched\nsource: openapi/optimizely-cmp-openapi.yml\ndocs: https://docs.developers.optimizely.com/web-experimentation/docs/registration\nschemes:\n- name: oauth2\n  source: openapi/optimizely-cmp-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.cmp.optimizely.com/oauth/token\n  description: OAuth 2.0 authentication for the CMP API.\nscopes:\n- scope: all\n  description: >-\n    The only supported scope for the Optimizely Web Experimentation REST API\n    OAuth 2.0 flow. The generated token has permissions that match the user\n    role of the authorizing user.\n  sources:\n  - https://docs.developers.optimizely.com/web-experimentation/docs/registration\n- scope: openid\n  description: >-\n    OpenID Connect scope used in the Optimizely CMP authorization code flow to\n    identify the user.\n  sources:\n  - https://docs.developers.optimizely.com/content-marketing-platform/docs/authentication-1\n- scope: profile\n\
  \  description: >-\n    OpenID Connect scope used in the Optimizely CMP authorization code flow to\n    access user profile information.\n  sources:\n  - https://docs.developers.optimizely.com/content-marketing-platform/docs/authentication-1\n- scope: offline_access\n  description: >-\n    OpenID Connect scope used in the Optimizely CMP authorization code flow to\n    obtain refresh tokens for long-lived access.\n  sources:\n  - https://docs.developers.optimizely.com/content-marketing-platform/docs/authentication-1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/scopes/optimizely-scopes.yml
summary_line: 4 scopes · clientCredentials
tags:
- A/B Testing
- Content Management
- Customer Data
- E-Commerce
- Experimentation
- Feature Flags
- Marketing
token_urls:
- https://api.cmp.optimizely.com/oauth/token
---
