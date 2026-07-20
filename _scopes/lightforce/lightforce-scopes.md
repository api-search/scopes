---
authorization_urls:
- https://id.lightforceortho.com/authorize
description: ''
docs: https://id.lightforceortho.com/.well-known/openid-configuration
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Lightforce Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Lightforce publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Lightforce API on a user''s behalf.


  Tokens are issued from https://id.lightforceortho.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Lightforce
provider_slug: lightforce
schemes:
- flows:
  - authorizationUrl: https://id.lightforceortho.com/authorize
    flow: authorizationCode
    tokenUrl: https://id.lightforceortho.com/oauth/token
  issuer: https://id.lightforceortho.com/
  name: OpenIDConnect
  source: well-known/lightforce-openid-configuration.json
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
- description: Request an ID token; required for OpenID Connect authentication.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows: []
  scope: profile
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: The user's full name claim.
  flows: []
  scope: name
- description: The user's given (first) name claim.
  flows: []
  scope: given_name
- description: The user's family (last) name claim.
  flows: []
  scope: family_name
- description: The user's nickname claim.
  flows: []
  scope: nickname
- description: The user's email address claim.
  flows: []
  scope: email
- description: Whether the user's email address has been verified.
  flows: []
  scope: email_verified
- description: The user's profile picture URL claim.
  flows: []
  scope: picture
- description: The timestamp the user record was created.
  flows: []
  scope: created_at
- description: Linked identity-provider identities for the user.
  flows: []
  scope: identities
- description: The user's phone number claim.
  flows: []
  scope: phone
- description: The user's address claim.
  flows: []
  scope: address
slug: lightforce-scopes
source_filename: lightforce-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://id.lightforceortho.com/.well-known/openid-configuration\ndocs: https://id.lightforceortho.com/.well-known/openid-configuration\nnotes: >-\n  Scopes are taken verbatim from `scopes_supported` in the live OIDC discovery document.\n  These are the standard OpenID Connect / Auth0 identity scopes — LightForce publishes\n  no product/API-resource scope reference, because there is no public LightForce API\n  behind this authorization server that outside developers can call. Treat this as the\n  identity scope surface only.\nschemes:\n- name: OpenIDConnect\n  source: well-known/lightforce-openid-configuration.json\n  issuer: https://id.lightforceortho.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.lightforceortho.com/authorize\n    tokenUrl: https://id.lightforceortho.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token; required for OpenID Connect authentication.\n  sources:\
  \ [well-known/lightforce-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims for the authenticated user.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: name\n  description: The user's full name claim.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: given_name\n  description: The user's given (first) name claim.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: family_name\n  description: The user's family (last) name claim.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: nickname\n  description: The user's nickname claim.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: email\n  description: The user's email address claim.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: email_verified\n\
  \  description: Whether the user's email address has been verified.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: picture\n  description: The user's profile picture URL claim.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: created_at\n  description: The timestamp the user record was created.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: identities\n  description: Linked identity-provider identities for the user.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: phone\n  description: The user's phone number claim.\n  sources: [well-known/lightforce-openid-configuration.json]\n- scope: address\n  description: The user's address claim.\n  sources: [well-known/lightforce-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightforce/refs/heads/main/scopes/lightforce-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Company
- Healthtech
- Orthodontics
- Dentistry
- Medical Devices
- 3D Printing
- Digital Manufacturing
- Identity
token_urls:
- https://id.lightforceortho.com/oauth/token
---
