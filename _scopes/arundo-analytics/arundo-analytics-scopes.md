---
authorization_urls:
- https://arundo.eu.auth0.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Arundo Analytics Scopes
name_suffix: OAuth Scopes
note: 'These are the scopes the Arundo Auth0 tenant advertises in its OIDC discovery document — the standard OpenID Connect identity scopes and claim-scopes. Arundo publishes NO API-resource scope vocabulary (no read:/write: style permissions), because the Foundation APIs have no public reference. Anything beyond this list would require an authenticated look at the tenant''s API (audience) definitions.'
overview: 'Arundo Analytics publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Arundo Analytics API on a user''s behalf.


  Tokens are issued from https://arundo.eu.auth0.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arundo Analytics
provider_slug: arundo-analytics
schemes:
- flows:
  - authorizationUrl: https://arundo.eu.auth0.com/authorize
    flow: authorizationCode
    tokenUrl: https://arundo.eu.auth0.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://arundo.eu.auth0.com/oauth/token
  - deviceAuthorizationUrl: https://arundo.eu.auth0.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://arundo.eu.auth0.com/oauth/token
  issuer: https://arundo.eu.auth0.com/
  name: OpenIDConnect
  source: well-known/arundo-analytics-openid-configuration.json
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
- created_at
- identities
- phone
- address
scopes:
- description: Request an ID token (OpenID Connect Core).
  flows: []
  scope: openid
- description: Access the end user's default profile claims.
  flows: []
  scope: profile
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: Access the end user's email address.
  flows: []
  scope: email
- description: Access whether the end user's email address has been verified.
  flows: []
  scope: email_verified
- description: Access the end user's full name claim.
  flows: []
  scope: name
- description: Access the end user's given name claim.
  flows: []
  scope: given_name
- description: Access the end user's family name claim.
  flows: []
  scope: family_name
- description: Access the end user's nickname claim.
  flows: []
  scope: nickname
- description: Access the end user's profile picture claim.
  flows: []
  scope: picture
- description: Access the end user's account creation timestamp claim.
  flows: []
  scope: created_at
- description: Access the end user's linked identity provider records.
  flows: []
  scope: identities
- description: Access the end user's phone number claim.
  flows: []
  scope: phone
- description: Access the end user's address claim.
  flows: []
  scope: address
slug: arundo-analytics-scopes
source_filename: arundo-analytics-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://arundo.eu.auth0.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  These are the scopes the Arundo Auth0 tenant advertises in its OIDC discovery\n  document — the standard OpenID Connect identity scopes and claim-scopes. Arundo\n  publishes NO API-resource scope vocabulary (no read:/write: style permissions),\n  because the Foundation APIs have no public reference. Anything beyond this list\n  would require an authenticated look at the tenant's API (audience) definitions.\nschemes:\n- name: OpenIDConnect\n  source: well-known/arundo-analytics-openid-configuration.json\n  issuer: https://arundo.eu.auth0.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://arundo.eu.auth0.com/authorize\n    tokenUrl: https://arundo.eu.auth0.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://arundo.eu.auth0.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://arundo.eu.auth0.com/oauth/device/code\n\
  \    tokenUrl: https://arundo.eu.auth0.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token (OpenID Connect Core).\n  kind: openid-connect\n- scope: profile\n  description: Access the end user's default profile claims.\n  kind: openid-connect\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  kind: openid-connect\n- scope: email\n  description: Access the end user's email address.\n  kind: openid-connect\n- scope: email_verified\n  description: Access whether the end user's email address has been verified.\n  kind: claim\n- scope: name\n  description: Access the end user's full name claim.\n  kind: claim\n- scope: given_name\n  description: Access the end user's given name claim.\n  kind: claim\n- scope: family_name\n  description: Access the end user's family name claim.\n  kind: claim\n- scope: nickname\n  description: Access the end user's nickname claim.\n  kind: claim\n- scope: picture\n  description: Access the end user's\
  \ profile picture claim.\n  kind: claim\n- scope: created_at\n  description: Access the end user's account creation timestamp claim.\n  kind: claim\n- scope: identities\n  description: Access the end user's linked identity provider records.\n  kind: claim\n- scope: phone\n  description: Access the end user's phone number claim.\n  kind: claim\n- scope: address\n  description: Access the end user's address claim.\n  kind: claim\ncoverage:\n  identity_scopes: 14\n  api_resource_scopes: 0\n  api_resource_scopes_note: not published — the Foundation API audiences are not publicly documented\nx-evidence:\n  fetched: '2026-08-06'\n  url: https://arundo.eu.auth0.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arundo-analytics/refs/heads/main/scopes/arundo-analytics-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Industrial AI
- Industrial IoT
- Analytics
- Machine-Learning
- Time Series
- Asset Performance Management
- Anomaly Detection
- Energy
- Maritime
- Oil and Gas
- Manufacturing
token_urls:
- https://arundo.eu.auth0.com/oauth/token
---
