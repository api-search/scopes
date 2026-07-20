---
authorization_urls: []
description: ''
docs: https://login.impartner.com/.well-known/openid-configuration
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Impartner Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Impartner publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Impartner API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Impartner
provider_slug: impartner
schemes:
- authorizationUrl: https://login.impartner.com/authorize
  issuer: https://login.impartner.com/
  name: OpenIDConnect
  source: well-known/impartner-openid-configuration.json
  tokenUrl: https://login.impartner.com/oauth/token
scope_count: 14
scope_names:
- openid
- profile
- email
- offline_access
- name
- given_name
- family_name
- nickname
- email_verified
- picture
- created_at
- identities
- phone
- address
scopes:
- description: OpenID Connect sign-in; returns an ID token.
  flows: []
  scope: openid
- description: Access to the user's basic profile claims (name, nickname, picture, etc.).
  flows: []
  scope: profile
- description: Access to the user's email and email_verified claims.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: User's full name claim.
  flows: []
  scope: name
- description: User's given (first) name claim.
  flows: []
  scope: given_name
- description: User's family (last) name claim.
  flows: []
  scope: family_name
- description: User's nickname claim.
  flows: []
  scope: nickname
- description: Whether the user's email has been verified.
  flows: []
  scope: email_verified
- description: User's profile picture URL.
  flows: []
  scope: picture
- description: Account creation timestamp claim.
  flows: []
  scope: created_at
- description: Linked identity provider identities.
  flows: []
  scope: identities
- description: User's phone number claim.
  flows: []
  scope: phone
- description: User's address claim.
  flows: []
  scope: address
slug: impartner-scopes
source_filename: impartner-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://login.impartner.com/.well-known/openid-configuration\ndocs: https://login.impartner.com/.well-known/openid-configuration\nschemes:\n- name: OpenIDConnect\n  source: well-known/impartner-openid-configuration.json\n  issuer: https://login.impartner.com/\n  authorizationUrl: https://login.impartner.com/authorize\n  tokenUrl: https://login.impartner.com/oauth/token\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; returns an ID token.\n- scope: profile\n  description: Access to the user's basic profile claims (name, nickname, picture, etc.).\n- scope: email\n  description: Access to the user's email and email_verified claims.\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n- scope: name\n  description: User's full name claim.\n- scope: given_name\n  description: User's given (first) name claim.\n- scope: family_name\n  description: User's family (last) name claim.\n\
  - scope: nickname\n  description: User's nickname claim.\n- scope: email_verified\n  description: Whether the user's email has been verified.\n- scope: picture\n  description: User's profile picture URL.\n- scope: created_at\n  description: Account creation timestamp claim.\n- scope: identities\n  description: Linked identity provider identities.\n- scope: phone\n  description: User's phone number claim.\n- scope: address\n  description: User's address claim.\nnotes:\n- These are the identity-tenant (Auth0) scopes advertised by the OIDC discovery document.\n- Fine-grained Impartner data-object permissions are governed per-tenant by roles, not by these OAuth scopes.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impartner/refs/heads/main/scopes/impartner-scopes.yml
summary_line: 14 scopes
tags:
- Company
- SaaS
- Partner Relationship Management
- PRM
- Channel Management
- Partner Ecosystem
- Through-Channel Marketing
- Sales
- CRM
token_urls: []
---
