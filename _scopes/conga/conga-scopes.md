---
authorization_urls:
- https://login.conga.com/authorize
description: ''
docs: https://developer.conga.com/platform/reference/authentication
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Conga Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Conga publishes 11 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Conga API on a user''s behalf.


  Tokens are issued from https://login.conga.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Conga
provider_slug: conga
schemes:
- flows:
  - authorizationUrl: https://login.conga.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.conga.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://login.conga.com/oauth/token
  issuer: https://login.conga.com/
  name: DeveloperPortalOIDC
  source: https://login.conga.com/.well-known/openid-configuration
scope_count: 11
scope_names:
- openid
- profile
- email
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- phone
- address
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows: []
  scope: openid
- description: Access to the user's default profile claims.
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
- description: User's profile picture claim.
  flows: []
  scope: picture
- description: User's phone number claim.
  flows: []
  scope: phone
- description: User's address claim.
  flows: []
  scope: address
slug: conga-scopes
source_filename: conga-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://login.conga.com/.well-known/openid-configuration\ndocs: https://developer.conga.com/platform/reference/authentication\nnotes: >-\n  Conga's REST API authorizes machine-to-machine calls with the OAuth 2.0\n  client_credentials grant; access is governed by the Integration User's platform\n  permissions rather than by fine-grained API scopes documented per operation.\n  The scopes below are the OIDC/identity scopes advertised by Conga's login\n  service (login.conga.com) discovery document. No per-resource API scope\n  reference is published in the developer docs.\nschemes:\n- name: DeveloperPortalOIDC\n  source: https://login.conga.com/.well-known/openid-configuration\n  issuer: https://login.conga.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.conga.com/authorize\n    tokenUrl: https://login.conga.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://login.conga.com/oauth/token\n\
  scopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n- scope: profile\n  description: Access to the user's default profile claims.\n- scope: email\n  description: Access to the user's email and email_verified claims.\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n- scope: name\n  description: User's full name claim.\n- scope: given_name\n  description: User's given (first) name claim.\n- scope: family_name\n  description: User's family (last) name claim.\n- scope: nickname\n  description: User's nickname claim.\n- scope: picture\n  description: User's profile picture claim.\n- scope: phone\n  description: User's phone number claim.\n- scope: address\n  description: User's address claim.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conga/refs/heads/main/scopes/conga-scopes.yml
summary_line: 11 scopes · authorizationCode/clientCredentials
tags:
- Company
- Enterprise Software
- Contract Lifecycle Management
- CPQ
- Revenue Lifecycle Management
- Document Automation
- E-Signature
- Contract Intelligence
- CRM
token_urls:
- https://login.conga.com/oauth/token
---
