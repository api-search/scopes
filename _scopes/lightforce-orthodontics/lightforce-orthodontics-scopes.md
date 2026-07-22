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
name: Lightforce Orthodontics Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'LightForce Orthodontics publishes 14 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the LightForce Orthodontics API on a user''s behalf.


  Tokens are issued from https://id.lightforceortho.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LightForce Orthodontics
provider_slug: lightforce-orthodontics
schemes:
- flows:
  - authorizationUrl: https://id.lightforceortho.com/authorize
    flow: authorizationCode
    tokenUrl: https://id.lightforceortho.com/oauth/token
  issuer: https://id.lightforceortho.com/
  name: LightForceOIDC
  source: well-known/lightforce-orthodontics-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- email
- email_verified
- name
- given_name
- family_name
- nickname
- picture
- phone
- address
- created_at
- identities
scopes:
- description: Request an ID token; indicates an OpenID Connect authentication request.
  flows: []
  scope: openid
- description: Access to the end-user's default profile claims.
  flows: []
  scope: profile
- description: Request a refresh token for access when the user is not present.
  flows: []
  scope: offline_access
- description: Access to the end-user's email address.
  flows: []
  scope: email
- description: Whether the end-user's email address has been verified.
  flows: []
  scope: email_verified
- description: End-user's full name.
  flows: []
  scope: name
- description: End-user's given (first) name.
  flows: []
  scope: given_name
- description: End-user's family (last) name.
  flows: []
  scope: family_name
- description: End-user's casual name.
  flows: []
  scope: nickname
- description: URL of the end-user's profile picture.
  flows: []
  scope: picture
- description: Access to the end-user's phone number.
  flows: []
  scope: phone
- description: Access to the end-user's postal address.
  flows: []
  scope: address
- description: Timestamp the end-user's account was created.
  flows: []
  scope: created_at
- description: Linked identity-provider identities for the end-user (Auth0 extension).
  flows: []
  scope: identities
slug: lightforce-orthodontics-scopes
source_filename: lightforce-orthodontics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://id.lightforceortho.com/.well-known/openid-configuration\ndocs: https://id.lightforceortho.com/.well-known/openid-configuration\nnotes: These are the scopes advertised by LightForce's Auth0 identity tenant via OIDC\n  discovery. They are the standard OpenID Connect scope and claim set — LightForce publishes\n  no product/API-specific scope reference, and no public API whose operations these would\n  authorize. Recorded as the real, verbatim advertised scope surface only.\nschemes:\n- name: LightForceOIDC\n  source: well-known/lightforce-orthodontics-openid-configuration.json\n  issuer: https://id.lightforceortho.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.lightforceortho.com/authorize\n    tokenUrl: https://id.lightforceortho.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token; indicates an OpenID Connect authentication request.\n  standard: openid-connect-core\n\
  - scope: profile\n  description: Access to the end-user's default profile claims.\n  standard: openid-connect-core\n- scope: offline_access\n  description: Request a refresh token for access when the user is not present.\n  standard: openid-connect-core\n- scope: email\n  description: Access to the end-user's email address.\n  standard: openid-connect-core\n- scope: email_verified\n  description: Whether the end-user's email address has been verified.\n- scope: name\n  description: End-user's full name.\n- scope: given_name\n  description: End-user's given (first) name.\n- scope: family_name\n  description: End-user's family (last) name.\n- scope: nickname\n  description: End-user's casual name.\n- scope: picture\n  description: URL of the end-user's profile picture.\n- scope: phone\n  description: Access to the end-user's phone number.\n  standard: openid-connect-core\n- scope: address\n  description: Access to the end-user's postal address.\n  standard: openid-connect-core\n- scope:\
  \ created_at\n  description: Timestamp the end-user's account was created.\n- scope: identities\n  description: Linked identity-provider identities for the end-user (Auth0 extension).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightforce-orthodontics/refs/heads/main/scopes/lightforce-orthodontics-scopes.yml
summary_line: 14 scopes · authorizationCode
tags:
- Company
- Healthcare
- Orthodontics
- Medical Devices
- Dental
- 3D Printing
- Manufacturing
- Identity
token_urls:
- https://id.lightforceortho.com/oauth/token
---
