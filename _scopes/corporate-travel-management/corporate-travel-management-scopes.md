---
authorization_urls:
- https://travelctm-au-production.au.auth0.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
- implicit
kind: oauth-scopes
layout: scope
method: searched
name: Corporate Travel Management Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Corporate Travel Management publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Corporate Travel Management API on a user''s behalf.


  Tokens are issued from https://travelctm-au-production.au.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Corporate Travel Management
provider_slug: corporate-travel-management
schemes:
- flows:
  - authorizationUrl: https://travelctm-au-production.au.auth0.com/authorize
    flow: authorizationCode
    pkce:
    - S256
    - plain
    tokenUrl: https://travelctm-au-production.au.auth0.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://travelctm-au-production.au.auth0.com/oauth/token
  - deviceAuthorizationUrl: https://travelctm-au-production.au.auth0.com/oauth/device/code
    flow: deviceCode
  - authorizationUrl: https://travelctm-au-production.au.auth0.com/authorize
    flow: implicit
  name: Auth0 OIDC (CTM Portal)
  source: well-known/corporate-travel-management-openid-configuration.json
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
- phone
- address
- created_at
- identities
scopes:
- description: Request an ID token (OpenID Connect).
  flows: []
  scope: openid
- description: Basic profile claims.
  flows: []
  scope: profile
- description: Email address claim.
  flows: []
  scope: email
- description: Email verification status claim.
  flows: []
  scope: email_verified
- description: Issue a refresh token.
  flows: []
  scope: offline_access
- description: Full name claim.
  flows: []
  scope: name
- description: Given name claim.
  flows: []
  scope: given_name
- description: Family name claim.
  flows: []
  scope: family_name
- description: Nickname claim.
  flows: []
  scope: nickname
- description: Profile picture claim.
  flows: []
  scope: picture
- description: Phone number claim.
  flows: []
  scope: phone
- description: Address claim.
  flows: []
  scope: address
- description: Account creation timestamp claim (Auth0 extension).
  flows: []
  scope: created_at
- description: Linked identity records claim (Auth0 extension).
  flows: []
  scope: identities
slug: corporate-travel-management-scopes
source_filename: corporate-travel-management-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: https://travelctm-au-production.au.auth0.com/.well-known/openid-configuration\ndocs: null\nsummary: >-\n  Corporate Travel Management publishes no scope or permission reference — there is no public API to\n  scope. The only scopes observable anywhere on a CTM property are the standard OpenID Connect\n  scopes and claim-scopes advertised by CTM's Auth0 tenant discovery document. They are Auth0/OIDC\n  defaults, not CTM-authored API permissions: no CTM resource scope (`read:bookings`,\n  `write:travellers`, …) is published, and the CTM Portal host API declares no\n  oauth-protected-resource metadata.\nschemes:\n- name: Auth0 OIDC (CTM Portal)\n  source: well-known/corporate-travel-management-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://travelctm-au-production.au.auth0.com/authorize\n    tokenUrl: https://travelctm-au-production.au.auth0.com/oauth/token\n    pkce: [S256, plain]\n\
  \  - flow: clientCredentials\n    tokenUrl: https://travelctm-au-production.au.auth0.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://travelctm-au-production.au.auth0.com/oauth/device/code\n  - flow: implicit\n    authorizationUrl: https://travelctm-au-production.au.auth0.com/authorize\nscopes:\n- scope: openid\n  description: Request an ID token (OpenID Connect).\n  kind: oidc-standard\n- scope: profile\n  description: Basic profile claims.\n  kind: oidc-standard\n- scope: email\n  description: Email address claim.\n  kind: oidc-standard\n- scope: email_verified\n  description: Email verification status claim.\n  kind: oidc-claim\n- scope: offline_access\n  description: Issue a refresh token.\n  kind: oidc-standard\n- scope: name\n  description: Full name claim.\n  kind: oidc-claim\n- scope: given_name\n  description: Given name claim.\n  kind: oidc-claim\n- scope: family_name\n  description: Family name claim.\n  kind: oidc-claim\n- scope: nickname\n  description:\
  \ Nickname claim.\n  kind: oidc-claim\n- scope: picture\n  description: Profile picture claim.\n  kind: oidc-claim\n- scope: phone\n  description: Phone number claim.\n  kind: oidc-standard\n- scope: address\n  description: Address claim.\n  kind: oidc-standard\n- scope: created_at\n  description: Account creation timestamp claim (Auth0 extension).\n  kind: auth0-extension\n- scope: identities\n  description: Linked identity records claim (Auth0 extension).\n  kind: auth0-extension\nctm_resource_scopes: []\nnotes: >-\n  Recorded because the discovery document is real and anonymously fetchable, not because CTM\n  operates a scoped API programme. Any CTM-defined API scopes would live on an Auth0 API (audience)\n  registration, which is not publicly enumerable.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corporate-travel-management/refs/heads/main/scopes/corporate-travel-management-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode/implicit
tags:
- Travel
- Australia
- Corporate Travel
- Travel Management Company
- Aviation
- NDC
- Distribution
- Booking
- Hotels
- Meetings and Events
token_urls:
- https://travelctm-au-production.au.auth0.com/oauth/token
---
