---
authorization_urls:
- https://tempus-ex.okta.com/oauth2/v1/authorize
description: ''
docs: https://docs.tempus-ex.com/fusionfeed/authentication
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Infinite Athlete Scopes
name_suffix: OAuth Scopes
note: FusionFeed authenticates OAuth2/OIDC bearer tokens issued by an external Okta tenant (https://tempus-ex.okta.com). The scopes below are the OIDC scopes the FusionFeed docs request during the Okta Authorization Code + PKCE flow, plus the additional scopes advertised by the Okta org authorization server discovery document. FusionFeed does not document its own API-resource scope namespace publicly; authorization to specific data is governed by the invited client's access policy embedded in the JWT.
overview: 'Infinite Athlete publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Infinite Athlete API on a user''s behalf.


  Tokens are issued from https://tempus-ex.okta.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Infinite Athlete
provider_slug: infinite-athlete
schemes:
- flows:
  - authorizationUrl: https://tempus-ex.okta.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://tempus-ex.okta.com/oauth2/v1/token
  name: OktaOAuth2
  source: https://docs.tempus-ex.com/fusionfeed/authentication
scope_count: 7
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- groups
scopes:
- description: OIDC authentication; required for the Authorization Code + PKCE flow.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Email claim.
  flows:
  - authorizationCode
  scope: email
- description: Address claim (advertised by the Okta authorization server).
  flows:
  - authorizationCode
  scope: address
- description: Phone claim (advertised by the Okta authorization server).
  flows:
  - authorizationCode
  scope: phone
- description: Refresh-token issuance (advertised by the Okta authorization server).
  flows:
  - authorizationCode
  scope: offline_access
- description: Group membership claim (advertised by the Okta authorization server).
  flows:
  - authorizationCode
  scope: groups
slug: infinite-athlete-scopes
source_filename: infinite-athlete-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.tempus-ex.com/fusionfeed/authentication\ndocs: https://docs.tempus-ex.com/fusionfeed/authentication\napi: FusionFeed\nnote: >-\n  FusionFeed authenticates OAuth2/OIDC bearer tokens issued by an external Okta\n  tenant (https://tempus-ex.okta.com). The scopes below are the OIDC scopes the\n  FusionFeed docs request during the Okta Authorization Code + PKCE flow, plus the\n  additional scopes advertised by the Okta org authorization server discovery\n  document. FusionFeed does not document its own API-resource scope namespace\n  publicly; authorization to specific data is governed by the invited client's\n  access policy embedded in the JWT.\nschemes:\n- name: OktaOAuth2\n  source: https://docs.tempus-ex.com/fusionfeed/authentication\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://tempus-ex.okta.com/oauth2/v1/authorize\n    tokenUrl: https://tempus-ex.okta.com/oauth2/v1/token\nscopes:\n- scope:\
  \ openid\n  description: OIDC authentication; required for the Authorization Code + PKCE flow.\n  flows: [authorizationCode]\n  sources: [docs, okta-discovery]\n- scope: profile\n  description: Basic profile claims.\n  flows: [authorizationCode]\n  sources: [docs, okta-discovery]\n- scope: email\n  description: Email claim.\n  flows: [authorizationCode]\n  sources: [docs, okta-discovery]\n- scope: address\n  description: Address claim (advertised by the Okta authorization server).\n  flows: [authorizationCode]\n  sources: [okta-discovery]\n- scope: phone\n  description: Phone claim (advertised by the Okta authorization server).\n  flows: [authorizationCode]\n  sources: [okta-discovery]\n- scope: offline_access\n  description: Refresh-token issuance (advertised by the Okta authorization server).\n  flows: [authorizationCode]\n  sources: [okta-discovery]\n- scope: groups\n  description: Group membership claim (advertised by the Okta authorization server).\n  flows: [authorizationCode]\n\
  \  sources: [okta-discovery]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinite-athlete/refs/heads/main/scopes/infinite-athlete-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Sports
- Sports Technology
- Sports Data
- Athlete Performance
- Biomechanics
- Video
- Real-Time Data
- Analytics
- GraphQL
token_urls:
- https://tempus-ex.okta.com/oauth2/v1/token
---
