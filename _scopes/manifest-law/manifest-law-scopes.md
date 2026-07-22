---
authorization_urls:
- https://app.manifestlaw.com/api/auth/oauth2/authorize
description: ''
docs: https://app.manifestlaw.com/.well-known/oauth-authorization-server
flows:
- authorizationCode
- clientCredentials
- refreshToken
kind: oauth-scopes
layout: scope
method: searched
name: Manifest Law Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Manifest Law publishes 7 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and refreshToken flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Manifest Law API on a user''s behalf.


  Tokens are issued from https://app.manifestlaw.com/api/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Manifest Law
provider_slug: manifest-law
schemes:
- flows:
  - authorizationUrl: https://app.manifestlaw.com/api/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://app.manifestlaw.com/api/auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://app.manifestlaw.com/api/auth/oauth2/token
  - flow: refreshToken
    tokenUrl: https://app.manifestlaw.com/api/auth/oauth2/token
  name: OAuth2
  source: well-known/manifest-law-oauth-authorization-server.json
scope_count: 7
scope_names:
- openid
- profile
- email
- offline_access
- api
- profile:full
- oauth_clients:manage
scopes:
- description: OpenID Connect authentication; issue an ID token.
  flows:
  - authorizationCode
  scope: openid
- description: Access basic profile claims (name, picture, given/family name).
  flows:
  - authorizationCode
  scope: profile
- description: Access the user's email and email_verified claims.
  flows:
  - authorizationCode
  scope: email
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  - refreshToken
  scope: offline_access
- description: Programmatic access to the Manifest Law (ManifestOS) API.
  flows:
  - authorizationCode
  - clientCredentials
  scope: api
- description: Access the full profile record.
  flows:
  - authorizationCode
  scope: profile:full
- description: Manage OAuth client registrations (dynamic client management).
  flows:
  - authorizationCode
  - clientCredentials
  scope: oauth_clients:manage
slug: manifest-law-scopes
source_filename: manifest-law-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://app.manifestlaw.com/.well-known/openid-configuration\ndocs: https://app.manifestlaw.com/.well-known/oauth-authorization-server\nschemes:\n- name: OAuth2\n  source: well-known/manifest-law-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.manifestlaw.com/api/auth/oauth2/authorize\n    tokenUrl: https://app.manifestlaw.com/api/auth/oauth2/token\n  - flow: clientCredentials\n    tokenUrl: https://app.manifestlaw.com/api/auth/oauth2/token\n  - flow: refreshToken\n    tokenUrl: https://app.manifestlaw.com/api/auth/oauth2/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issue an ID token.\n  flows: [authorizationCode]\n  sources: [well-known/manifest-law-openid-configuration.json]\n- scope: profile\n  description: Access basic profile claims (name, picture, given/family name).\n  flows: [authorizationCode]\n  sources: [well-known/manifest-law-openid-configuration.json]\n\
  - scope: email\n  description: Access the user's email and email_verified claims.\n  flows: [authorizationCode]\n  sources: [well-known/manifest-law-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  flows: [authorizationCode, refreshToken]\n  sources: [well-known/manifest-law-openid-configuration.json]\n- scope: api\n  description: Programmatic access to the Manifest Law (ManifestOS) API.\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/manifest-law-openid-configuration.json]\n- scope: profile:full\n  description: Access the full profile record.\n  flows: [authorizationCode]\n  sources: [well-known/manifest-law-openid-configuration.json]\n- scope: oauth_clients:manage\n  description: Manage OAuth client registrations (dynamic client management).\n  flows: [authorizationCode, clientCredentials]\n  sources: [well-known/manifest-law-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manifest-law/refs/heads/main/scopes/manifest-law-scopes.yml
summary_line: 7 scopes · authorizationCode/clientCredentials/refreshToken
tags:
- Company
- Legal
- Legal Tech
- Case Management
- Communication
- OAuth
- OpenID Connect
token_urls:
- https://app.manifestlaw.com/api/auth/oauth2/token
---
