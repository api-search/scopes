---
authorization_urls:
- https://auth.eagleeyenetworks.com/oauth2/authorize
description: ''
docs: https://developer.eagleeyenetworks.com/recipes/oauth-authentication
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Eagle Eye Networks Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Eagle Eye Networks publishes 4 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Eagle Eye Networks API on a user''s behalf.


  Tokens are issued from https://auth.eagleeyenetworks.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Eagle Eye Networks
provider_slug: eagle-eye-networks
schemes:
- flows:
  - authorizationUrl: https://auth.eagleeyenetworks.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token
  name: OAuth2
  source: well-known/eagle-eye-networks-openid-configuration.json
scope_count: 4
scope_names:
- vms.all
- openid
- profile
- email
scopes:
- description: Full access to the Eagle Eye Video API Platform (v3); the scope used across the documented OAuth authorization-code and client-credentials examples.
  flows:
  - authorizationCode
  - clientCredentials
  scope: vms.all
- description: OpenID Connect authentication; returns an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the end user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access to the end user's email claim.
  flows:
  - authorizationCode
  scope: email
slug: eagle-eye-networks-scopes
source_filename: eagle-eye-networks-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.eagleeyenetworks.com/.well-known/openid-configuration\ndocs: https://developer.eagleeyenetworks.com/recipes/oauth-authentication\nschemes:\n- name: OAuth2\n  source: well-known/eagle-eye-networks-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.eagleeyenetworks.com/oauth2/authorize\n    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.eagleeyenetworks.com/oauth2/token\nscopes:\n- scope: vms.all\n  description: Full access to the Eagle Eye Video API Platform (v3); the scope used\n    across the documented OAuth authorization-code and client-credentials examples.\n  flows:\n  - authorizationCode\n  - clientCredentials\n  sources:\n  - https://developer.eagleeyenetworks.com/recipes/oauth-authentication\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  flows:\n \
  \ - authorizationCode\n  sources:\n  - well-known/eagle-eye-networks-openid-configuration.json\n- scope: profile\n  description: Access to the end user's basic profile claims.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/eagle-eye-networks-openid-configuration.json\n- scope: email\n  description: Access to the end user's email claim.\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/eagle-eye-networks-openid-configuration.json\nnotes: >-\n  Eagle Eye's public documentation presents a single coarse API scope, vms.all,\n  granting full Video API Platform access; the OIDC scopes openid/profile/email\n  come from the authorization-server discovery document. Fine-grained authorization\n  is enforced by account type, user roles, permissions, and resource grants rather\n  than by additional OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eagle-eye-networks/refs/heads/main/scopes/eagle-eye-networks-scopes.yml
summary_line: 4 scopes · authorizationCode/clientCredentials
tags:
- Company
- Security
- Video Surveillance
- Video Management
- Cloud Video
- Cameras
- Physical Security
- Video Analytics
- License Plate Recognition
- Streaming
- Webhooks
- OAuth
token_urls:
- https://auth.eagleeyenetworks.com/oauth2/token
---
