---
authorization_urls:
- https://login.bpsnap.com/authorize
description: ''
docs: https://login.bpsnap.com/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
kind: oauth-scopes
layout: scope
method: searched
name: Blackpoint Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Blackpoint publishes 6 OAuth 2.0 scopes via the authorizationCode and clientCredentials flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Blackpoint API on a user''s behalf.


  Tokens are issued from https://login.bpsnap.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Blackpoint
provider_slug: blackpoint
schemes:
- flows:
  - authorizationUrl: https://login.bpsnap.com/authorize
    flow: authorizationCode
    tokenUrl: https://login.bpsnap.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://login.bpsnap.com/oauth/token
  name: CompassOneOIDC
  source: https://login.bpsnap.com/.well-known/openid-configuration
scope_count: 6
scope_names:
- openid
- profile
- email
- offline_access
- roles
- groups
scopes:
- description: OpenID Connect sign-in; issue an ID token.
  flows: []
  scope: openid
- description: Access to the user's basic profile claims.
  flows: []
  scope: profile
- description: Access to the user's email address and verification status.
  flows: []
  scope: email
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: Include the user's CompassOne roles in the token (Auth0 custom scope).
  flows: []
  scope: roles
- description: Include the user's group memberships in the token (Auth0 custom scope).
  flows: []
  scope: groups
slug: blackpoint-scopes
source_filename: blackpoint-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://login.bpsnap.com/.well-known/openid-configuration\ndocs: https://login.bpsnap.com/.well-known/openid-configuration\nnotes: >-\n  Blackpoint CompassOne authenticates through an Auth0 OIDC tenant\n  (login.bpsnap.com). Scopes below are the standard OIDC/Auth0 scopes advertised\n  by the tenant's discovery document, plus the runtime scope string the\n  CompassOne web app requests. Fine-grained CompassOne API permission scopes are\n  not published on a public reference page (the product API at\n  api.blackpointcyber.com is gated).\nschemes:\n- name: CompassOneOIDC\n  source: https://login.bpsnap.com/.well-known/openid-configuration\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.bpsnap.com/authorize\n    tokenUrl: https://login.bpsnap.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://login.bpsnap.com/oauth/token\nruntime_scope_request: \"openid profile email roles groups offline_access\"\
  \nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; issue an ID token.\n- scope: profile\n  description: Access to the user's basic profile claims.\n- scope: email\n  description: Access to the user's email address and verification status.\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n- scope: roles\n  description: Include the user's CompassOne roles in the token (Auth0 custom scope).\n- scope: groups\n  description: Include the user's group memberships in the token (Auth0 custom scope).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackpoint/refs/heads/main/scopes/blackpoint-scopes.yml
summary_line: 6 scopes · authorizationCode/clientCredentials
tags:
- Company
- Cybersecurity
- Managed Detection and Response
- MDR
- Security Operations
- Identity Threat Detection
- Security Posture Management
- MSP
- SIEM
token_urls:
- https://login.bpsnap.com/oauth/token
---
