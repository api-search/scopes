---
authorization_urls:
- https://sso.plbtech.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Premialab Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PremiaLab publishes 7 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PremiaLab API on a user''s behalf.


  Tokens are issued from https://sso.plbtech.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PremiaLab
provider_slug: premialab
schemes:
- flows:
  - authorizationUrl: https://sso.plbtech.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://sso.plbtech.com/oauth2/v1/token
  name: PremiaLabOAuth2
  source: well-known/premialab-openid-configuration.json
scope_count: 7
scope_names:
- openid
- email
- profile
- address
- phone
- offline_access
- groups
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows: []
  scope: openid
- description: Access to the user's email address and verification status.
  flows: []
  scope: email
- description: Access to the user's basic profile claims (name, locale, etc.).
  flows: []
  scope: profile
- description: Access to the user's address claim.
  flows: []
  scope: address
- description: Access to the user's phone number and verification status.
  flows: []
  scope: phone
- description: Issue a refresh token for long-lived, offline access.
  flows: []
  scope: offline_access
- description: Access to the user's group/role memberships.
  flows: []
  scope: groups
slug: premialab-scopes
source_filename: premialab-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://sso.plbtech.com/.well-known/openid-configuration\nnotes: >-\n  Scopes advertised by the PremiaLab Tech (Okta) OIDC authorization server that\n  fronts https://api.premialab.com. These are the standard OpenID Connect scopes\n  exposed by the issuer's default authorization server; any product-specific API\n  scopes are provisioned per institutional client and are not publicly published.\nschemes:\n  - name: PremiaLabOAuth2\n    source: well-known/premialab-openid-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sso.plbtech.com/oauth2/v1/authorize\n        tokenUrl: https://sso.plbtech.com/oauth2/v1/token\nscopes:\n  - scope: openid\n    description: OpenID Connect authentication; returns an ID token.\n    sources: [well-known/premialab-openid-configuration.json]\n  - scope: email\n    description: Access to the user's email address and verification status.\n    sources:\
  \ [well-known/premialab-openid-configuration.json]\n  - scope: profile\n    description: Access to the user's basic profile claims (name, locale, etc.).\n    sources: [well-known/premialab-openid-configuration.json]\n  - scope: address\n    description: Access to the user's address claim.\n    sources: [well-known/premialab-openid-configuration.json]\n  - scope: phone\n    description: Access to the user's phone number and verification status.\n    sources: [well-known/premialab-openid-configuration.json]\n  - scope: offline_access\n    description: Issue a refresh token for long-lived, offline access.\n    sources: [well-known/premialab-openid-configuration.json]\n  - scope: groups\n    description: Access to the user's group/role memberships.\n    sources: [well-known/premialab-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/premialab/refs/heads/main/scopes/premialab-scopes.yml
summary_line: 7 scopes · authorizationCode
tags:
- Company
- Financial Services
- Fintech
- Investment Management
- Risk Analytics
- Portfolio Analytics
- Quantitative Investment Strategies
- Factor Investing
token_urls:
- https://sso.plbtech.com/oauth2/v1/token
---
