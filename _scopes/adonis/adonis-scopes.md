---
authorization_urls:
- https://auth.adonis.io/authorize
description: ''
docs: https://adonis.io/platform
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Adonis Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Adonis publishes 14 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Adonis API on a user''s behalf.


  Tokens are issued from https://auth.adonis.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Adonis
provider_slug: adonis
schemes:
- flows:
  - authorizationUrl: https://auth.adonis.io/authorize
    flow: authorizationCode
    tokenUrl: https://auth.adonis.io/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.adonis.io/oauth/token
  issuer: https://auth.adonis.io/
  name: OpenIDConnect
  source: well-known/adonis-openid-configuration.json
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
- description: Request an OpenID Connect ID token for authentication.
  flows:
  - authorizationCode
  scope: openid
- description: Access the end user's default profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Access the end user's name.
  flows:
  - authorizationCode
  scope: name
- description: Access the end user's given (first) name.
  flows:
  - authorizationCode
  scope: given_name
- description: Access the end user's family (last) name.
  flows:
  - authorizationCode
  scope: family_name
- description: Access the end user's nickname.
  flows:
  - authorizationCode
  scope: nickname
- description: Access the end user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Access the end user's email verification status.
  flows:
  - authorizationCode
  scope: email_verified
- description: Access the end user's profile picture.
  flows:
  - authorizationCode
  scope: picture
- description: Access the timestamp the end user's account was created.
  flows:
  - authorizationCode
  scope: created_at
- description: Access the end user's linked identity providers.
  flows:
  - authorizationCode
  scope: identities
- description: Access the end user's phone number.
  flows:
  - authorizationCode
  scope: phone
- description: Access the end user's address.
  flows:
  - authorizationCode
  scope: address
slug: adonis-scopes
source_filename: adonis-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://auth.adonis.io/.well-known/openid-configuration\ndocs: https://adonis.io/platform\nschemes:\n- name: OpenIDConnect\n  source: well-known/adonis-openid-configuration.json\n  issuer: https://auth.adonis.io/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.adonis.io/authorize\n    tokenUrl: https://auth.adonis.io/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.adonis.io/oauth/token\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token for authentication.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: profile\n  description: Access the end user's default profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n\
  - scope: name\n  description: Access the end user's name.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: given_name\n  description: Access the end user's given (first) name.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: family_name\n  description: Access the end user's family (last) name.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: nickname\n  description: Access the end user's nickname.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: email\n  description: Access the end user's email address.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: email_verified\n  description: Access the end user's email verification status.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: picture\n  description:\
  \ Access the end user's profile picture.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: created_at\n  description: Access the timestamp the end user's account was created.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: identities\n  description: Access the end user's linked identity providers.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: phone\n  description: Access the end user's phone number.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\n- scope: address\n  description: Access the end user's address.\n  flows: [authorizationCode]\n  sources: [well-known/adonis-openid-configuration.json]\nnotes: >-\n  Scopes are the standard OpenID Connect / Auth0 identity scopes advertised in\n  the discovery document's scopes_supported. Adonis application- and\n  resource-specific API scopes (RCM, eligibility,\
  \ claims) are provisioned per\n  Auth0 API/audience and are not published in the public discovery document.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adonis/refs/heads/main/scopes/adonis-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials
tags:
- Company
- Healthcare
- Revenue Cycle Management
- RCM
- Medical Billing
- Health IT
- Eligibility Verification
- Claims
- Payments
- Artificial Intelligence
- Automation
token_urls:
- https://auth.adonis.io/oauth/token
---
