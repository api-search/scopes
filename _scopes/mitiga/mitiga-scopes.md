---
authorization_urls:
- https://api.mitiga.cloud/oauth-2/authorize
description: The only scopes Mitiga advertises anonymously are the standard OpenID Connect and Auth0 profile-claim scopes carried in the authorization-server metadata on its API host. No product-specific scopes (alerts, investigations, data lake, response actions) are published; those would require authenticated introspection of a customer tenant. Recorded honestly rather than inferred.
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Mitiga Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Mitiga publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Mitiga API on a user''s behalf.


  Tokens are issued from https://api.mitiga.cloud/oauth-2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Mitiga
provider_slug: mitiga
schemes:
- flows:
  - authorizationUrl: https://api.mitiga.cloud/oauth-2/authorize
    flow: authorizationCode
    tokenUrl: https://api.mitiga.cloud/oauth-2/token
  - flow: clientCredentials
    tokenUrl: https://api.mitiga.cloud/oauth-2/token
  - deviceAuthorizationUrl: https://auth.mitiga.cloud/oauth/device/code
    flow: deviceCode
    tokenUrl: https://api.mitiga.cloud/oauth-2/token
  name: oauth2
  source: well-known/mitiga-oauth-authorization-server.json
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
- description: Request an ID token — OpenID Connect authentication.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
- description: The user's email address.
  flows: []
  scope: email
- description: Whether the user's email address has been verified.
  flows: []
  scope: email_verified
- description: The user's full name claim.
  flows: []
  scope: name
- description: The user's given name claim.
  flows: []
  scope: given_name
- description: The user's family name claim.
  flows: []
  scope: family_name
- description: The user's nickname claim.
  flows: []
  scope: nickname
- description: The user's profile picture URL claim.
  flows: []
  scope: picture
- description: The account creation timestamp claim.
  flows: []
  scope: created_at
- description: Linked identity-provider identities for the user.
  flows: []
  scope: identities
- description: The user's phone number claims.
  flows: []
  scope: phone
- description: The user's address claim.
  flows: []
  scope: address
slug: mitiga-scopes
source_filename: mitiga-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://api.mitiga.cloud/.well-known/oauth-authorization-server\ndocs: null\ndescription: >-\n  The only scopes Mitiga advertises anonymously are the standard OpenID Connect and\n  Auth0 profile-claim scopes carried in the authorization-server metadata on its API\n  host. No product-specific scopes (alerts, investigations, data lake, response actions)\n  are published; those would require authenticated introspection of a customer tenant.\n  Recorded honestly rather than inferred.\nschemes:\n- name: oauth2\n  source: well-known/mitiga-oauth-authorization-server.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.mitiga.cloud/oauth-2/authorize\n    tokenUrl: https://api.mitiga.cloud/oauth-2/token\n  - flow: clientCredentials\n    tokenUrl: https://api.mitiga.cloud/oauth-2/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.mitiga.cloud/oauth/device/code\n    tokenUrl: https://api.mitiga.cloud/oauth-2/token\n\
  scopes:\n- scope: openid\n  description: Request an ID token — OpenID Connect authentication.\n  standard: true\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: profile\n  description: Basic profile claims for the authenticated user.\n  standard: true\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  standard: true\n  flows: [authorizationCode, deviceCode]\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: email\n  description: The user's email address.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: email_verified\n  description: Whether the user's email address has been verified.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: name\n  description: The user's full name\
  \ claim.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: given_name\n  description: The user's given name claim.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: family_name\n  description: The user's family name claim.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: nickname\n  description: The user's nickname claim.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: picture\n  description: The user's profile picture URL claim.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: created_at\n  description: The account creation timestamp claim.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: identities\n  description: Linked identity-provider identities for the user.\n  standard: false\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n\
  - scope: phone\n  description: The user's phone number claims.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\n- scope: address\n  description: The user's address claim.\n  standard: true\n  sources: [well-known/mitiga-oauth-authorization-server.json]\ngaps:\n- >-\n  No product/resource scopes are published. An integrator cannot tell from the public\n  surface what a client_credentials token is authorized to do against the Mitiga platform.\nx-evidence:\n- url: https://api.mitiga.cloud/.well-known/oauth-authorization-server\n  http_status: 200\n  fetched: '2026-08-04'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mitiga/refs/heads/main/scopes/mitiga-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Security
- Cloud Security
- SaaS Security
- Cloud Detection and Response
- Incident Response
- Threat Detection
- Identity Security
- Managed Security Services
- Artificial Intelligence
token_urls:
- https://api.mitiga.cloud/oauth-2/token
---
