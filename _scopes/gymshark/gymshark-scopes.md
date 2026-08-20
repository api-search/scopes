---
authorization_urls:
- https://auth.gymshark.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- implicit
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Gymshark Scopes
name_suffix: OAuth Scopes
note: Read verbatim from the `scopes_supported` array of Gymshark's own OpenID Connect Discovery document. Gymshark publishes no scope/permission reference page, so there are no product- or resource-level scopes to add — every scope advertised here is a standard OpenID Connect / Auth0 identity scope covering the customer profile, not a Gymshark business API. Scope descriptions below are the OpenID Connect Core 1.0 §5.4 / Auth0 definitions of these standard scopes, not Gymshark-authored copy.
overview: 'Gymshark publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, implicit, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gymshark API on a user''s behalf.


  Tokens are issued from https://auth.gymshark.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gymshark
provider_slug: gymshark
schemes:
- flows:
  - authorizationUrl: https://auth.gymshark.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.gymshark.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.gymshark.com/oauth/token
  - authorizationUrl: https://auth.gymshark.com/authorize
    flow: implicit
  - deviceAuthorizationUrl: https://auth.gymshark.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.gymshark.com/oauth/token
  issuer: https://auth.gymshark.com/
  name: gymshark-oidc
  source: well-known/gymshark-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- name
- given_name
- family_name
- nickname
- email
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Request an ID token and perform OpenID Connect authentication.
  flows: []
  scope: openid
- description: Request the default profile claims (name, family_name, given_name, nickname, picture, created_at).
  flows: []
  scope: profile
- description: Request a refresh token so the client can obtain new access tokens without the user present.
  flows: []
  scope: offline_access
- description: Request the `name` claim.
  flows: []
  scope: name
- description: Request the `given_name` claim.
  flows: []
  scope: given_name
- description: Request the `family_name` claim.
  flows: []
  scope: family_name
- description: Request the `nickname` claim.
  flows: []
  scope: nickname
- description: Request the `email` claim.
  flows: []
  scope: email
- description: Request the `email_verified` claim.
  flows: []
  scope: email_verified
- description: Request the `picture` claim.
  flows: []
  scope: picture
- description: Request the account `created_at` claim.
  flows: []
  scope: created_at
- description: Request the linked-identity array for the account (Auth0 extension).
  flows: []
  scope: identities
- description: Request the `phone_number` and `phone_number_verified` claims.
  flows: []
  scope: phone
- description: Request the `address` claim.
  flows: []
  scope: address
slug: gymshark-scopes
source_filename: gymshark-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://auth.gymshark.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Read verbatim from the `scopes_supported` array of Gymshark's own OpenID Connect\n  Discovery document. Gymshark publishes no scope/permission reference page, so there\n  are no product- or resource-level scopes to add — every scope advertised here is a\n  standard OpenID Connect / Auth0 identity scope covering the customer profile, not a\n  Gymshark business API. Scope descriptions below are the OpenID Connect Core 1.0 §5.4\n  / Auth0 definitions of these standard scopes, not Gymshark-authored copy.\nschemes:\n- name: gymshark-oidc\n  source: well-known/gymshark-openid-configuration.json\n  issuer: https://auth.gymshark.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.gymshark.com/authorize\n    tokenUrl: https://auth.gymshark.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.gymshark.com/oauth/token\n\
  \  - flow: implicit\n    authorizationUrl: https://auth.gymshark.com/authorize\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.gymshark.com/oauth/device/code\n    tokenUrl: https://auth.gymshark.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token and perform OpenID Connect authentication.\n  standard: OpenID Connect Core 1.0\n- scope: profile\n  description: Request the default profile claims (name, family_name, given_name, nickname,\n    picture, created_at).\n  standard: OpenID Connect Core 1.0\n- scope: offline_access\n  description: Request a refresh token so the client can obtain new access tokens without\n    the user present.\n  standard: OpenID Connect Core 1.0\n- scope: name\n  description: Request the `name` claim.\n- scope: given_name\n  description: Request the `given_name` claim.\n- scope: family_name\n  description: Request the `family_name` claim.\n- scope: nickname\n  description: Request the `nickname` claim.\n- scope: email\n\
  \  description: Request the `email` claim.\n  standard: OpenID Connect Core 1.0\n- scope: email_verified\n  description: Request the `email_verified` claim.\n- scope: picture\n  description: Request the `picture` claim.\n- scope: created_at\n  description: Request the account `created_at` claim.\n- scope: identities\n  description: Request the linked-identity array for the account (Auth0 extension).\n- scope: phone\n  description: Request the `phone_number` and `phone_number_verified` claims.\n  standard: OpenID Connect Core 1.0\n- scope: address\n  description: Request the `address` claim.\n  standard: OpenID Connect Core 1.0\ncoverage:\n  scopes_total: 14\n  resource_scopes: 0\n  identity_scopes: 14\nx-evidence:\n  fetched: '2026-08-04'\n  url: https://auth.gymshark.com/.well-known/openid-configuration\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gymshark/refs/heads/main/scopes/gymshark-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/implicit/deviceCode
tags:
- Company
- Retail
- E-Commerce
- Apparel
- Fitness
- Consumer
- Direct to Consumer
- Identity
- OpenID Connect
token_urls:
- https://auth.gymshark.com/oauth/token
---
