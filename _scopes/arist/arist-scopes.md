---
authorization_urls:
- https://auth.arist.app/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Arist Scopes
name_suffix: OAuth Scopes
note: Arist publishes no OpenAPI and no product-level permission/scope reference, so these are the scopes advertised by its own OIDC authorization server (an Auth0 tenant on the auth.arist.app hostname). They are the standard OIDC / Auth0 claim-release scope set — identity scopes, not Arist product scopes. No documented scope governs access to the gated platform API at api.arist.app.
overview: 'Arist publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Arist API on a user''s behalf.


  Tokens are issued from https://auth.arist.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Arist
provider_slug: arist
schemes:
- flows:
  - authorizationUrl: https://auth.arist.app/authorize
    flow: authorizationCode
    tokenUrl: https://auth.arist.app/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.arist.app/oauth/token
  - deviceAuthorizationUrl: https://auth.arist.app/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.arist.app/oauth/token
  issuer: https://auth.arist.app/
  name: AristOIDC
  source: well-known/arist-openid-configuration.json
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
- description: Request an ID token — the base OpenID Connect scope.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Release the standard profile claims for the authenticated user.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Issue a refresh token so the client can renew access without user presence.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
- description: Release the user's full name claim.
  flows:
  - authorizationCode
  scope: name
- description: Release the user's given name claim.
  flows:
  - authorizationCode
  scope: given_name
- description: Release the user's family name claim.
  flows:
  - authorizationCode
  scope: family_name
- description: Release the user's nickname claim.
  flows:
  - authorizationCode
  scope: nickname
- description: Release the user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Release whether the user's email address has been verified.
  flows:
  - authorizationCode
  scope: email_verified
- description: Release the user's profile picture URL.
  flows:
  - authorizationCode
  scope: picture
- description: Release the timestamp the user record was created.
  flows:
  - authorizationCode
  scope: created_at
- description: Release the linked identity-provider identities for the user.
  flows:
  - authorizationCode
  scope: identities
- description: Release the user's phone number claims.
  flows:
  - authorizationCode
  scope: phone
- description: Release the user's address claim.
  flows:
  - authorizationCode
  scope: address
slug: arist-scopes
source_filename: arist-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://auth.arist.app/.well-known/openid-configuration\nnote: |\n  Arist publishes no OpenAPI and no product-level permission/scope reference, so these are\n  the scopes advertised by its own OIDC authorization server (an Auth0 tenant on the\n  auth.arist.app hostname). They are the standard OIDC / Auth0 claim-release scope set —\n  identity scopes, not Arist product scopes. No documented scope governs access to the\n  gated platform API at api.arist.app.\nschemes:\n- name: AristOIDC\n  issuer: https://auth.arist.app/\n  source: well-known/arist-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.arist.app/authorize\n    tokenUrl: https://auth.arist.app/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.arist.app/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.arist.app/oauth/device/code\n    tokenUrl: https://auth.arist.app/oauth/token\n\
  scopes:\n- scope: openid\n  description: Request an ID token — the base OpenID Connect scope.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: profile\n  description: Release the standard profile claims for the authenticated user.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can renew access without user presence.\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: name\n  description: Release the user's full name claim.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: given_name\n  description: Release the user's given name claim.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: family_name\n  description: Release the user's family name claim.\n \
  \ flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: nickname\n  description: Release the user's nickname claim.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: email\n  description: Release the user's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: email_verified\n  description: Release whether the user's email address has been verified.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: picture\n  description: Release the user's profile picture URL.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: created_at\n  description: Release the timestamp the user record was created.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: identities\n  description: Release the linked identity-provider\
  \ identities for the user.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: phone\n  description: Release the user's phone number claims.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\n- scope: address\n  description: Release the user's address claim.\n  flows: [authorizationCode]\n  sources: [well-known/arist-openid-configuration.json]\nx-evidence:\n  fetched: '2026-08-02'\n  url: https://auth.arist.app/.well-known/openid-configuration\n  http_status: 200\n  scope_count: 14\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arist/refs/heads/main/scopes/arist-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Learning
- Training
- Enablement
- Microlearning
- Human Resources
- Messaging
- Artificial Intelligence
- Employee Communications
- SaaS
token_urls:
- https://auth.arist.app/oauth/token
---
