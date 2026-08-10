---
authorization_urls:
- https://auth.recurohealth.com/authorize
description: ''
docs: https://auth.recurohealth.com/.well-known/openid-configuration
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Recuro Health Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Recuro Health publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Recuro Health API on a user''s behalf.


  Tokens are issued from https://auth.recurohealth.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Recuro Health
provider_slug: recuro-health
schemes:
- flows:
  - authorizationUrl: https://auth.recurohealth.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.recurohealth.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.recurohealth.com/oauth/token
  - deviceAuthorizationUrl: https://auth.recurohealth.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.recurohealth.com/oauth/token
  issuer: https://auth.recurohealth.com/
  name: OpenIDConnect
  source: well-known/recuro-health-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- offline_access
- email
- address
- phone
- name
- given_name
- family_name
- nickname
- email_verified
- picture
- created_at
- identities
scopes:
- description: Requests an ID token; required to initiate an OpenID Connect authentication.
  flows: []
  scope: openid
- description: Basic profile claims for the authenticated end user.
  flows: []
  scope: profile
- description: Requests a refresh token so the client can obtain new access tokens without the user present.
  flows: []
  scope: offline_access
- description: The end user's email address claim.
  flows: []
  scope: email
- description: The end user's postal address claim.
  flows: []
  scope: address
- description: The end user's phone number claim.
  flows: []
  scope: phone
- description: The end user's full name claim.
  flows: []
  scope: name
- description: The end user's given name claim.
  flows: []
  scope: given_name
- description: The end user's family name claim.
  flows: []
  scope: family_name
- description: The end user's nickname claim.
  flows: []
  scope: nickname
- description: Whether the end user's email address has been verified.
  flows: []
  scope: email_verified
- description: URL of the end user's profile picture.
  flows: []
  scope: picture
- description: Timestamp the end user's account was created.
  flows: []
  scope: created_at
- description: The linked identity providers associated with the end user.
  flows: []
  scope: identities
slug: recuro-health-scopes
source_filename: recuro-health-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://auth.recurohealth.com/.well-known/openid-configuration\ndocs: https://auth.recurohealth.com/.well-known/openid-configuration\nnotes: >-\n  Every scope below is taken verbatim from the `scopes_supported` array Recuro Health\n  publishes in its own OpenID Connect discovery document. These are the standard OIDC\n  scopes and claim-scopes advertised by the authorization server; Recuro Health publishes\n  no API-resource (audience-specific) scopes anywhere public, so none are recorded here.\n  Nothing in this file is inferred.\nschemes:\n- name: OpenIDConnect\n  source: well-known/recuro-health-openid-configuration.json\n  issuer: https://auth.recurohealth.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.recurohealth.com/authorize\n    tokenUrl: https://auth.recurohealth.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.recurohealth.com/oauth/token\n  - flow: deviceCode\n\
  \    deviceAuthorizationUrl: https://auth.recurohealth.com/oauth/device/code\n    tokenUrl: https://auth.recurohealth.com/oauth/token\nscopes:\n- scope: openid\n  description: Requests an ID token; required to initiate an OpenID Connect authentication.\n  kind: oidc-core\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: profile\n  description: Basic profile claims for the authenticated end user.\n  kind: oidc-core\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: offline_access\n  description: Requests a refresh token so the client can obtain new access tokens without\n    the user present.\n  kind: oidc-core\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: email\n  description: The end user's email address claim.\n  kind: oidc-core\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: address\n  description: The end user's postal address claim.\n  kind: oidc-core\n  sources:\n\
  \  - well-known/recuro-health-openid-configuration.json\n- scope: phone\n  description: The end user's phone number claim.\n  kind: oidc-core\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: name\n  description: The end user's full name claim.\n  kind: claim\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: given_name\n  description: The end user's given name claim.\n  kind: claim\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: family_name\n  description: The end user's family name claim.\n  kind: claim\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: nickname\n  description: The end user's nickname claim.\n  kind: claim\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: email_verified\n  description: Whether the end user's email address has been verified.\n  kind: claim\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope:\
  \ picture\n  description: URL of the end user's profile picture.\n  kind: claim\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: created_at\n  description: Timestamp the end user's account was created.\n  kind: claim\n  sources:\n  - well-known/recuro-health-openid-configuration.json\n- scope: identities\n  description: The linked identity providers associated with the end user.\n  kind: claim\n  sources:\n  - well-known/recuro-health-openid-configuration.json\ncoverage:\n  scopes_total: 14\n  resource_scopes: 0\n  gap: >-\n    No API-resource scopes are published. Recuro Health's protected resource APIs are not\n    publicly documented, so the authorization model beyond OIDC identity cannot be read\n    from any public surface.\nx-evidence:\n  fetched: '2026-08-05'\n  url: https://auth.recurohealth.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recuro-health/refs/heads/main/scopes/recuro-health-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Health
- Healthcare
- Telehealth
- Virtual Care
- Digital Health
- Behavioral Health
- Primary Care
- Employee Benefits
- Health Plans
- Identity
- OpenID Connect
token_urls:
- https://auth.recurohealth.com/oauth/token
---
