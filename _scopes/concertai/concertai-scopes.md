---
authorization_urls:
- https://auth.precision.concertai.com/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: probed
name: Concertai Scopes
name_suffix: OAuth Scopes
note: ConcertAI publishes no scopes or permissions reference. The scopes below are the scopes_supported advertised by the OpenID Connect discovery document on the Auth0 tenant fronting the Precision platform. They are the standard OIDC claim scopes plus offline_access — no product/resource scopes (data, trial, imaging, patient) are advertised anonymously, which means any API-level authorization model for the Precision or Eureka platforms is not publicly discoverable.
overview: 'ConcertAI publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the ConcertAI API on a user''s behalf.


  Tokens are issued from https://auth.precision.concertai.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ConcertAI
provider_slug: concertai
schemes:
- flows:
  - authorizationUrl: https://auth.precision.concertai.com/authorize
    flow: authorizationCode
    tokenUrl: https://auth.precision.concertai.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.precision.concertai.com/oauth/token
  - deviceAuthorizationUrl: https://auth.precision.concertai.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.precision.concertai.com/oauth/token
  issuer: https://auth.precision.concertai.com/
  name: precision-oidc
  source: well-known/concertai-precision-openid-configuration.json
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
- description: Request an OpenID Connect ID token for the authenticating user.
  flows:
  - authorizationCode
  scope: openid
- description: Access the user's basic profile claims.
  flows:
  - authorizationCode
  scope: profile
- description: Issue a refresh token for long-lived access.
  flows:
  - authorizationCode
  scope: offline_access
- description: Access the user's full name claim.
  flows:
  - authorizationCode
  scope: name
- description: Access the user's given name claim.
  flows:
  - authorizationCode
  scope: given_name
- description: Access the user's family name claim.
  flows:
  - authorizationCode
  scope: family_name
- description: Access the user's nickname claim.
  flows:
  - authorizationCode
  scope: nickname
- description: Access the user's email address claim.
  flows:
  - authorizationCode
  scope: email
- description: Access the user's email verification status claim.
  flows:
  - authorizationCode
  scope: email_verified
- description: Access the user's profile picture claim.
  flows:
  - authorizationCode
  scope: picture
- description: Access the account creation timestamp claim.
  flows:
  - authorizationCode
  scope: created_at
- description: Access the linked-identity claim for federated accounts.
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
slug: concertai-scopes
source_filename: concertai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: https://auth.precision.concertai.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  ConcertAI publishes no scopes or permissions reference. The scopes below are the\n  scopes_supported advertised by the OpenID Connect discovery document on the Auth0\n  tenant fronting the Precision platform. They are the standard OIDC claim scopes plus\n  offline_access — no product/resource scopes (data, trial, imaging, patient) are\n  advertised anonymously, which means any API-level authorization model for the\n  Precision or Eureka platforms is not publicly discoverable.\nschemes:\n- name: precision-oidc\n  source: well-known/concertai-precision-openid-configuration.json\n  issuer: https://auth.precision.concertai.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.precision.concertai.com/authorize\n    tokenUrl: https://auth.precision.concertai.com/oauth/token\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://auth.precision.concertai.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.precision.concertai.com/oauth/device/code\n    tokenUrl: https://auth.precision.concertai.com/oauth/token\nscopes:\n- scope: openid\n  description: Request an OpenID Connect ID token for the authenticating user.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: profile\n  description: Access the user's basic profile claims.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: name\n  description: Access the user's full name claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: given_name\n  description: Access\
  \ the user's given name claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: family_name\n  description: Access the user's family name claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: nickname\n  description: Access the user's nickname claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: email\n  description: Access the user's email address claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: email_verified\n  description: Access the user's email verification status claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: picture\n  description: Access the user's profile picture claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n\
  - scope: created_at\n  description: Access the account creation timestamp claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: identities\n  description: Access the linked-identity claim for federated accounts.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: phone\n  description: Access the user's phone number claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\n- scope: address\n  description: Access the user's address claim.\n  flows: [authorizationCode]\n  sources: [well-known/concertai-precision-openid-configuration.json]\nx-evidence:\n- url: https://auth.precision.concertai.com/.well-known/openid-configuration\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concertai/refs/heads/main/scopes/concertai-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Company
- Healthcare
- Oncology
- Artificial Intelligence
- Real-World Data
- Clinical Trials
- Life Sciences
- Medical Imaging
- Health Data
token_urls:
- https://auth.precision.concertai.com/oauth/token
---
