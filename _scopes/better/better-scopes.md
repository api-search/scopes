---
authorization_urls:
- https://prod.bettermg.com/api/idp/sso
description: ''
docs: https://better.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Better Scopes
name_suffix: OAuth Scopes
note: OIDC scopes advertised by the consumer sign-in identity provider (AWS Cognito). These are standard OpenID Connect scopes, not developer-API permission scopes; Better publishes no public developer API.
overview: 'Better publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Better API on a user''s behalf.


  Tokens are issued from https://prod.bettermg.com/api/idp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Better
provider_slug: better
schemes:
- flows:
  - authorizationUrl: https://prod.bettermg.com/api/idp/sso
    flow: authorizationCode
    tokenUrl: https://prod.bettermg.com/api/idp/token
  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_ZQ2HayNPw
  name: BetterOIDC
  source: well-known/better-openid-configuration.json
scope_count: 4
scope_names:
- openid
- email
- phone
- profile
scopes:
- description: OpenID Connect authentication; issue an ID token for the signed-in user.
  flows:
  - authorizationCode
  scope: openid
- description: Access to the user's email address and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Access to the user's phone_number and phone_number_verified claims.
  flows:
  - authorizationCode
  scope: phone
- description: Access to the user's default profile claims (name, etc.).
  flows:
  - authorizationCode
  scope: profile
slug: better-scopes
source_filename: better-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: well-known/better-openid-configuration.json\ndocs: https://better.com/.well-known/openid-configuration\nnote: >-\n  OIDC scopes advertised by the consumer sign-in identity provider (AWS Cognito).\n  These are standard OpenID Connect scopes, not developer-API permission scopes;\n  Better publishes no public developer API.\nschemes:\n- name: BetterOIDC\n  source: well-known/better-openid-configuration.json\n  issuer: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_ZQ2HayNPw\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://prod.bettermg.com/api/idp/sso\n    tokenUrl: https://prod.bettermg.com/api/idp/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token for the signed-in user.\n  flows: [authorizationCode]\n  sources: [well-known/better-openid-configuration.json]\n- scope: email\n  description: Access to the user's email address and email_verified claims.\n\
  \  flows: [authorizationCode]\n  sources: [well-known/better-openid-configuration.json]\n- scope: phone\n  description: Access to the user's phone_number and phone_number_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/better-openid-configuration.json]\n- scope: profile\n  description: Access to the user's default profile claims (name, etc.).\n  flows: [authorizationCode]\n  sources: [well-known/better-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/better/refs/heads/main/scopes/better-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- Mortgage
- Lending
- Fintech
- Real Estate
- Home Equity
- Insurance
- Financial Services
token_urls:
- https://prod.bettermg.com/api/idp/token
---
