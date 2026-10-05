---
authorization_urls: []
description: ''
docs: https://developer.sygnum.com/client-management
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Sygnum Scopes
name_suffix: OAuth Scopes
note: Two scope surfaces exist and only one of them is public. The OIDC scopes below are the identity scopes the Auth0 tenant advertises anonymously. The API scopes that actually gate the Banking/Trading/Custody/Staking/Connect/Protect/Market Data resources are served from https://api.sygnum.com/b2b/v1/available-scopes, which returns HTTP 401 to an anonymous caller — they are enumerable only inside the developer portal's Access Management screen after a client login. Nothing about the API scope names is asserted here because nothing about them is published.
overview: 'Sygnum publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Sygnum API on a user''s behalf.


  Tokens are issued from https://auth.sygnum.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Sygnum
provider_slug: sygnum
schemes: []
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
- description: OIDC — issue an ID token for the authenticated subject.
  flows: []
  scope: openid
- description: OIDC — basic profile claims.
  flows: []
  scope: profile
- description: OIDC — issue a refresh token.
  flows: []
  scope: offline_access
- description: OIDC — email address claim.
  flows: []
  scope: email
- description: OIDC — email verification status claim.
  flows: []
  scope: email_verified
- description: OIDC — full name claim.
  flows: []
  scope: name
- description: OIDC — given name claim.
  flows: []
  scope: given_name
- description: OIDC — family name claim.
  flows: []
  scope: family_name
- description: OIDC — nickname claim.
  flows: []
  scope: nickname
- description: OIDC — profile picture claim.
  flows: []
  scope: picture
- description: OIDC — account creation timestamp claim.
  flows: []
  scope: created_at
- description: Auth0 — linked identity providers claim.
  flows: []
  scope: identities
- description: OIDC — phone number claim.
  flows: []
  scope: phone
- description: OIDC — postal address claim.
  flows: []
  scope: address
slug: sygnum-scopes
source_filename: sygnum-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://auth.sygnum.com/.well-known/openid-configuration (HTTP 200)\nnote: >-\n  Two scope surfaces exist and only one of them is public. The OIDC scopes below are the\n  identity scopes the Auth0 tenant advertises anonymously. The API scopes that actually\n  gate the Banking/Trading/Custody/Staking/Connect/Protect/Market Data resources are served\n  from https://api.sygnum.com/b2b/v1/available-scopes, which returns HTTP 401 to an\n  anonymous caller — they are enumerable only inside the developer portal's Access\n  Management screen after a client login. Nothing about the API scope names is asserted\n  here because nothing about them is published.\ndocs: https://developer.sygnum.com/client-management\nauthorization_server: https://auth.sygnum.com/\ntoken_endpoint: https://auth.sygnum.com/oauth/token\nscopes:\n- name: openid\n  description: OIDC — issue an ID token for the authenticated subject.\n- name: profile\n  description:\
  \ OIDC — basic profile claims.\n- name: offline_access\n  description: OIDC — issue a refresh token.\n- name: email\n  description: OIDC — email address claim.\n- name: email_verified\n  description: OIDC — email verification status claim.\n- name: name\n  description: OIDC — full name claim.\n- name: given_name\n  description: OIDC — given name claim.\n- name: family_name\n  description: OIDC — family name claim.\n- name: nickname\n  description: OIDC — nickname claim.\n- name: picture\n  description: OIDC — profile picture claim.\n- name: created_at\n  description: OIDC — account creation timestamp claim.\n- name: identities\n  description: Auth0 — linked identity providers claim.\n- name: phone\n  description: OIDC — phone number claim.\n- name: address\n  description: OIDC — postal address claim.\napi_scopes:\n  published: false\n  endpoint: https://api.sygnum.com/b2b/v1/available-scopes\n  http_status: 401\n  assignment: >-\n    Per Auth0 client, chosen in the developer portal when\
  \ the client is created or edited\n    (\"New Auth0 client -> Scope\"), and bound to the partner's contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sygnum/refs/heads/main/scopes/sygnum-scopes.yml
summary_line: 14 scopes
tags:
- Company
- Banking
- Digital Assets
- Cryptocurrency
- Custody
- Trading
- Staking
- Tokenization
- Settlement
- Market Data
- Financial Services
- Switzerland
- Singapore
- B2B
token_bound: false
token_urls:
- https://auth.sygnum.com/oauth/token
---
