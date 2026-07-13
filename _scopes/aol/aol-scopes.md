---
api_specs:
- filename: aol-openapi.yml
  format: yaml
  label: Yahoo Developer Network (formerly AOL Developer)
  slug: yahoo-developer-network-formerly-aol-developer
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/openapi/aol-openapi.yml
authorization_urls:
- https://api.login.yahoo.com/oauth2/request_auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Aol Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'AOL publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the AOL API on a user''s behalf.


  Tokens are issued from https://api.login.yahoo.com/oauth2/get_token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AOL
provider_slug: aol
schemes:
- flows:
  - authorizationUrl: https://api.login.yahoo.com/oauth2/request_auth
    flow: authorizationCode
    tokenUrl: https://api.login.yahoo.com/oauth2/get_token
  name: oauth2
  source: openapi/aol-openapi.yml
scope_count: 3
scope_names:
- email
- openid
- profile
scopes:
- description: Email address
  flows:
  - authorizationCode
  scope: email
- description: OpenID Connect authentication
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile information
  flows:
  - authorizationCode
  scope: profile
slug: aol-scopes
source_filename: aol-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aol-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/aol-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.login.yahoo.com/oauth2/request_auth\n    tokenUrl: https://api.login.yahoo.com/oauth2/get_token\nscopes:\n- scope: email\n  description: Email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aol-openapi.yml\n- scope: openid\n  description: OpenID Connect authentication\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aol-openapi.yml\n- scope: profile\n  description: Basic profile information\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/aol-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aol/refs/heads/main/scopes/aol-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Advertising
- Digital Media
- Entertainment
- News
- Fortune 1000
token_urls:
- https://api.login.yahoo.com/oauth2/get_token
---
