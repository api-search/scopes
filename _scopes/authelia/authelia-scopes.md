---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Authelia REST API
  slug: authelia-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/authelia/authelia/master/api/openapi.yml
authorization_urls:
- https://auth.example.com/api/oidc/authorization
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Authelia Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Authelia publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Authelia API on a user''s behalf.


  Tokens are issued from https://auth.example.com/api/oidc/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Authelia
provider_slug: authelia
schemes:
- flows:
  - authorizationUrl: https://auth.example.com/api/oidc/authorization
    flow: authorizationCode
    tokenUrl: https://auth.example.com/api/oidc/token
  name: oauth2
  source: openapi/authelia-openapi.yml
scope_count: 5
scope_names:
- email
- groups
- offline_access
- openid
- profile
scopes:
- description: Email claims
  flows:
  - authorizationCode
  scope: email
- description: Group memberships
  flows:
  - authorizationCode
  scope: groups
- description: Refresh token
  flows:
  - authorizationCode
  scope: offline_access
- description: OpenID Connect base scope
  flows:
  - authorizationCode
  scope: openid
- description: Profile claims
  flows:
  - authorizationCode
  scope: profile
slug: authelia-scopes
source_filename: authelia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/authelia-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/authelia-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.example.com/api/oidc/authorization\n    tokenUrl: https://auth.example.com/api/oidc/token\nscopes:\n- scope: email\n  description: Email claims\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/authelia-openapi.yml\n- scope: groups\n  description: Group memberships\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/authelia-openapi.yml\n- scope: offline_access\n  description: Refresh token\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/authelia-openapi.yml\n- scope: openid\n  description: OpenID Connect base scope\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/authelia-openapi.yml\n- scope: profile\n  description: Profile claims\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/authelia-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authelia/refs/heads/main/scopes/authelia-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Authentication
- Authorization
- LDAP
- MFA
- Open Source
- OpenID Connect
- Self-Hosted
- SSO
token_urls:
- https://auth.example.com/api/oidc/token
---
