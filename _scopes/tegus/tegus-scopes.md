---
authorization_urls:
- https://auth.tegus.com/authorize
description: ''
docs: https://auth.tegus.com/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Tegus Scopes
name_suffix: OAuth Scopes
note: These are the scopes advertised by the Tegus identity provider's OIDC discovery document (scopes_supported). They are the standard OpenID Connect / Auth0 identity scopes — Tegus publishes no product API scope reference, because the Tegus developer hub is retired (tegus.readme.io -> /inactive) and the API surface moved to AlphaSense. No API-resource scopes are asserted here; none are published.
overview: 'Tegus publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Tegus API on a user''s behalf.


  Tokens are issued from https://auth.tegus.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Tegus
provider_slug: tegus
schemes:
- flows:
  - authorizationUrl: https://auth.tegus.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.tegus.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.tegus.com/oauth/token
  - deviceAuthorizationUrl: https://auth.tegus.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.tegus.com/oauth/token
  issuer: https://auth.tegus.com/
  name: TegusOAuth2
  source: well-known/tegus-openid-configuration.json
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
- description: Request an ID token; signals an OpenID Connect authentication request.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticated user.
  flows: []
  scope: profile
- description: Issue a refresh token so the client can act after the access token expires.
  flows: []
  scope: offline_access
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
- description: The user's email address claim.
  flows: []
  scope: email
- description: Whether the user's email address has been verified.
  flows: []
  scope: email_verified
- description: The user's profile picture URL.
  flows: []
  scope: picture
- description: When the user account was created.
  flows: []
  scope: created_at
- description: The linked identity-provider connections for the user.
  flows: []
  scope: identities
- description: The user's phone number claim.
  flows: []
  scope: phone
- description: The user's address claim.
  flows: []
  scope: address
slug: tegus-scopes
source_filename: tegus-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: https://auth.tegus.com/.well-known/openid-configuration\ndocs: https://auth.tegus.com/.well-known/openid-configuration\nnote: >-\n  These are the scopes advertised by the Tegus identity provider's OIDC discovery\n  document (scopes_supported). They are the standard OpenID Connect / Auth0 identity\n  scopes — Tegus publishes no product API scope reference, because the Tegus developer\n  hub is retired (tegus.readme.io -> /inactive) and the API surface moved to AlphaSense.\n  No API-resource scopes are asserted here; none are published.\nschemes:\n- name: TegusOAuth2\n  source: well-known/tegus-openid-configuration.json\n  issuer: https://auth.tegus.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.tegus.com/authorize\n    tokenUrl: https://auth.tegus.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.tegus.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.tegus.com/oauth/device/code\n\
  \    tokenUrl: https://auth.tegus.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token; signals an OpenID Connect authentication request.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims for the authenticated user.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token so the client can act after the access token expires.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: name\n  description: The user's full name claim.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: given_name\n  description: The user's given name claim.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: family_name\n  description: The user's family name claim.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n\
  - scope: nickname\n  description: The user's nickname claim.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: email\n  description: The user's email address claim.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: email_verified\n  description: Whether the user's email address has been verified.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: picture\n  description: The user's profile picture URL.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: created_at\n  description: When the user account was created.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: identities\n  description: The linked identity-provider connections for the user.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n- scope: phone\n  description: The user's phone number claim.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\n\
  - scope: address\n  description: The user's address claim.\n  kind: identity\n  sources: [well-known/tegus-openid-configuration.json]\ncoverage:\n  identity_scopes: 14\n  api_resource_scopes: 0\n  api_resource_scopes_note: >-\n    No product API audience or resource scopes are published at any public Tegus URL.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://auth.tegus.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tegus/refs/heads/main/scopes/tegus-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Investment Research
- Expert Networks
- Market Intelligence
- Financial Data
- Transcripts
- Private Markets
- Equity Research
- OpenID Connect
- Acquired
token_urls:
- https://auth.tegus.com/oauth/token
---
