---
authorization_urls: []
description: ''
docs: https://api.echo3d.com/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Echo3D Scopes
name_suffix: OAuth Scopes
note: These OAuth/OIDC scopes govern the echo3D console/dashboard identity provider (Auth0 tenant echo3d.us.auth0.com), advertised via OIDC discovery on api.echo3d.com. The RESTful data API (upload/query/download/delete) does NOT use OAuth scopes — it authenticates with key + email + userKey. These are the standard OIDC scopes exposed by the identity provider, not data-plane permissions.
overview: 'echo3D publishes 14 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the echo3D API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: echo3D
provider_slug: echo3d
schemes:
- authorizationUrl: https://echo3d.us.auth0.com/authorize
  flows:
  - authorizationCode
  - clientCredentials
  issuer: https://echo3d.us.auth0.com/
  name: ConsoleOIDC
  tokenUrl: https://echo3d.us.auth0.com/oauth/token
scope_count: 14
scope_names:
- openid
- profile
- email
- email_verified
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- created_at
- identities
- phone
- address
scopes:
- description: Authenticate the user and return an ID token (OIDC).
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Access the user's email address.
  flows:
  - authorizationCode
  scope: email
- description: Access the user's email-verification status.
  flows:
  - authorizationCode
  scope: email_verified
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Access the user's full name claim.
  flows:
  - authorizationCode
  scope: name
- description: Access the user's given (first) name.
  flows:
  - authorizationCode
  scope: given_name
- description: Access the user's family (last) name.
  flows:
  - authorizationCode
  scope: family_name
- description: Access the user's nickname claim.
  flows:
  - authorizationCode
  scope: nickname
- description: Access the user's profile picture URL.
  flows:
  - authorizationCode
  scope: picture
- description: Access the user account creation timestamp.
  flows:
  - authorizationCode
  scope: created_at
- description: Access linked identity provider records for the user.
  flows:
  - authorizationCode
  scope: identities
- description: Access the user's phone number claim.
  flows:
  - authorizationCode
  scope: phone
- description: Access the user's address claim.
  flows:
  - authorizationCode
  scope: address
slug: echo3d-scopes
source_filename: echo3d-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.echo3d.com/.well-known/openid-configuration\ndocs: https://api.echo3d.com/.well-known/openid-configuration\nnote: >-\n  These OAuth/OIDC scopes govern the echo3D console/dashboard identity provider\n  (Auth0 tenant echo3d.us.auth0.com), advertised via OIDC discovery on\n  api.echo3d.com. The RESTful data API (upload/query/download/delete) does NOT\n  use OAuth scopes — it authenticates with key + email + userKey. These are the\n  standard OIDC scopes exposed by the identity provider, not data-plane\n  permissions.\nschemes:\n- name: ConsoleOIDC\n  issuer: https://echo3d.us.auth0.com/\n  authorizationUrl: https://echo3d.us.auth0.com/authorize\n  tokenUrl: https://echo3d.us.auth0.com/oauth/token\n  flows:\n  - authorizationCode\n  - clientCredentials\nscopes:\n- scope: openid\n  description: Authenticate the user and return an ID token (OIDC).\n  flows: [authorizationCode]\n- scope: profile\n  description: Access\
  \ the user's basic profile claims.\n  flows: [authorizationCode]\n- scope: email\n  description: Access the user's email address.\n  flows: [authorizationCode]\n- scope: email_verified\n  description: Access the user's email-verification status.\n  flows: [authorizationCode]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  flows: [authorizationCode]\n- scope: name\n  description: Access the user's full name claim.\n  flows: [authorizationCode]\n- scope: given_name\n  description: Access the user's given (first) name.\n  flows: [authorizationCode]\n- scope: family_name\n  description: Access the user's family (last) name.\n  flows: [authorizationCode]\n- scope: nickname\n  description: Access the user's nickname claim.\n  flows: [authorizationCode]\n- scope: picture\n  description: Access the user's profile picture URL.\n  flows: [authorizationCode]\n- scope: created_at\n  description: Access the user account creation timestamp.\n  flows: [authorizationCode]\n\
  - scope: identities\n  description: Access linked identity provider records for the user.\n  flows: [authorizationCode]\n- scope: phone\n  description: Access the user's phone number claim.\n  flows: [authorizationCode]\n- scope: address\n  description: Access the user's address claim.\n  flows: [authorizationCode]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/echo3d/refs/heads/main/scopes/echo3d-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials
tags:
- Company
- 3D
- Augmented Reality
- Virtual Reality
- Digital Asset Management
- 3D Models
- Content Delivery
- Developer Tools
- SDKs
- WebAR
token_urls: []
---
