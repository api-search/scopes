---
authorization_urls:
- https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Flow Engineering Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Flow Engineering publishes 4 OAuth 2.0 scopes via the authorizationCode and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Flow Engineering API on a user''s behalf.


  Tokens are issued from https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Flow Engineering
provider_slug: flow-engineering
schemes:
- flows:
  - authorizationUrl: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/token
  - authorizationUrl: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/authorize
    flow: implicit
  name: Cognito OAuth2 / OIDC
  source: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_iODQDOUFS/.well-known/openid-configuration
scope_count: 4
scope_names:
- openid
- email
- phone
- profile
scopes:
- description: OpenID Connect authentication; returns the subject identifier in the ID token.
  flows:
  - authorizationCode
  - implicit
  scope: openid
- description: Access to the user's email address and email_verified claim.
  flows:
  - authorizationCode
  - implicit
  scope: email
- description: Access to the user's phone number and phone_number_verified claim.
  flows:
  - authorizationCode
  - implicit
  scope: phone
- description: Access to the user's standard profile claims (name, etc.).
  flows:
  - authorizationCode
  - implicit
  scope: profile
slug: flow-engineering-scopes
source_filename: flow-engineering-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_iODQDOUFS/.well-known/openid-configuration\nschemes:\n- name: Cognito OAuth2 / OIDC\n  source: https://cognito-idp.eu-west-2.amazonaws.com/eu-west-2_iODQDOUFS/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/authorize\n    tokenUrl: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/token\n  - flow: implicit\n    authorizationUrl: https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/authorize\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns the subject identifier in the ID token.\n  flows: [authorizationCode, implicit]\n- scope: email\n  description: Access to the user's email address and email_verified claim.\n  flows: [authorizationCode, implicit]\n- scope: phone\n  description: Access to the user's phone\
  \ number and phone_number_verified claim.\n  flows: [authorizationCode, implicit]\n- scope: profile\n  description: Access to the user's standard profile claims (name, etc.).\n  flows: [authorizationCode, implicit]\nnotes: >-\n  scopes_supported reflects the standard OIDC scopes advertised by the Cognito user pool\n  discovery document. Any Flow-specific resource-server scopes are not advertised at the pool\n  discovery endpoint and would require the documented enterprise onboarding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flow-engineering/refs/heads/main/scopes/flow-engineering-scopes.yml
summary_line: 4 scopes · authorizationCode/implicit
tags:
- Company
- Software Development
- Hardware Engineering
- Requirements Management
- Systems Engineering
- MBSE
- AI Agents
- CAD
- Product Lifecycle Management
- GraphQL
token_urls:
- https://flowengineering.auth.eu-west-2.amazoncognito.com/oauth2/token
---
