---
authorization_urls:
- https://auth.evertune.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- implicit
kind: oauth-scopes
layout: scope
method: probed
name: Evertune Scopes
name_suffix: OAuth Scopes
note: These are the scopes_supported advertised by Evertune's Auth0 tenant at auth.evertune.ai. They are the standard OpenID Connect identity/profile scopes plus Auth0's offline_access -- they govern sign-in to the Evertune web application, not access to any product API. Evertune publishes no developer API and therefore no API permission/scope reference; there is no scopes or permissions page on evertune.ai or docs.evertune.ai to search. Recorded verbatim from the discovery document, with nothing added.
overview: 'Evertune publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Evertune API on a user''s behalf.


  Tokens are issued from https://auth.evertune.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Evertune
provider_slug: evertune
schemes:
- flows:
  - authorizationUrl: https://auth.evertune.ai/authorize
    flow: authorizationCode
    tokenUrl: https://auth.evertune.ai/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.evertune.ai/oauth/token
  - authorizationUrl: https://auth.evertune.ai/authorize
    flow: implicit
  issuer: https://auth.evertune.ai/
  name: Auth0OIDC
  source: well-known/evertune-openid-configuration.json
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
- description: OpenID Connect authentication; issues an ID token for the signed-in user.
  flows: []
  scope: openid
- description: Basic profile claims for the signed-in user.
  flows: []
  scope: profile
- description: Issues a refresh token for long-lived sessions.
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
- description: The user's profile picture claim.
  flows: []
  scope: picture
- description: When the user account was created.
  flows: []
  scope: created_at
- description: The linked identity providers for the user account.
  flows: []
  scope: identities
- description: The user's phone number claim.
  flows: []
  scope: phone
- description: The user's address claim.
  flows: []
  scope: address
slug: evertune-scopes
source_filename: evertune-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://auth.evertune.ai/.well-known/openid-configuration\ndocs: null\nnote: >-\n  These are the scopes_supported advertised by Evertune's Auth0 tenant at\n  auth.evertune.ai. They are the standard OpenID Connect identity/profile\n  scopes plus Auth0's offline_access -- they govern sign-in to the Evertune web\n  application, not access to any product API. Evertune publishes no developer\n  API and therefore no API permission/scope reference; there is no scopes or\n  permissions page on evertune.ai or docs.evertune.ai to search. Recorded\n  verbatim from the discovery document, with nothing added.\nschemes:\n- name: Auth0OIDC\n  source: well-known/evertune-openid-configuration.json\n  issuer: https://auth.evertune.ai/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.evertune.ai/authorize\n    tokenUrl: https://auth.evertune.ai/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://auth.evertune.ai/oauth/token\n\
  \  - flow: implicit\n    authorizationUrl: https://auth.evertune.ai/authorize\nscope_count: 14\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; issues an ID token for the signed-in user.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: profile\n  description: Basic profile claims for the signed-in user.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: offline_access\n  description: Issues a refresh token for long-lived sessions.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: name\n  description: The user's full name claim.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: given_name\n  description: The user's given name claim.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: family_name\n  description: The user's family name claim.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n\
  - scope: nickname\n  description: The user's nickname claim.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: email\n  description: The user's email address claim.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: email_verified\n  description: Whether the user's email address has been verified.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: picture\n  description: The user's profile picture claim.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: created_at\n  description: When the user account was created.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: identities\n  description: The linked identity providers for the user account.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\n- scope: phone\n  description: The user's phone number claim.\n  layer: identity\n\
  \  sources: [well-known/evertune-openid-configuration.json]\n- scope: address\n  description: The user's address claim.\n  layer: identity\n  sources: [well-known/evertune-openid-configuration.json]\napi_scopes: []\napi_scopes_note: >-\n  No product/API scopes are published. Evertune ships no developer API, so no\n  audience-bound scopes (read:*, write:*) exist to record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evertune/refs/heads/main/scopes/evertune-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/implicit
tags:
- Company
- Generative Engine Optimization
- AI Search
- Brand Monitoring
- Marketing Intelligence
- AI Visibility
- Analytics
- Artificial Intelligence
token_urls:
- https://auth.evertune.ai/oauth/token
---
