---
authorization_urls:
- https://auth.coadjute.com/authorize
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
name: Lifetise Scopes
name_suffix: OAuth Scopes
note: 'These are the scopes advertised by Coadjute''s Auth0 identity tenant — the standard OpenID Connect scope set plus Auth0''s per-claim scopes. They are the real, publicly fetchable scope surface, but they describe identity claims, NOT the authorization model of the Coadjute Network''s Partner Cloud API. No Coadjute product/API scopes are published anywhere public: api.coadjute.com answers 401 to every anonymous request and developer.coadjute.com (which once carried an API Catalogue) returns 502. Do not read this list as the network''s permission model.'
overview: 'Coadjute publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, deviceCode, and implicit flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Coadjute API on a user''s behalf.


  Tokens are issued from https://auth.coadjute.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Coadjute
provider_slug: lifetise
schemes:
- flows:
  - authorizationUrl: https://auth.coadjute.com/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://auth.coadjute.com/oauth/token
  - flow: clientCredentials
    tokenUrl: https://auth.coadjute.com/oauth/token
  - deviceAuthorizationUrl: https://auth.coadjute.com/oauth/device/code
    flow: deviceCode
    tokenUrl: https://auth.coadjute.com/oauth/token
  - authorizationUrl: https://auth.coadjute.com/authorize
    flow: implicit
  issuer: https://auth.coadjute.com/
  name: coadjute-oidc
  source: well-known/lifetise-openid-configuration.json
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
- description: Request an ID token — baseline OpenID Connect authentication.
  flows: []
  scope: openid
- description: Access the end user's default profile claims.
  flows: []
  scope: profile
- description: Issue a refresh token for long-lived access.
  flows: []
  scope: offline_access
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
- description: Access the end user's email address claim.
  flows: []
  scope: email
- description: Access whether the end user's email address has been verified.
  flows: []
  scope: email_verified
- description: Access the end user's profile picture claim.
  flows: []
  scope: picture
- description: Access the end user's account creation timestamp (Auth0 claim).
  flows: []
  scope: created_at
- description: Access the end user's linked identity providers (Auth0 claim).
  flows: []
  scope: identities
- description: Access the end user's phone number claim.
  flows: []
  scope: phone
- description: Access the end user's address claim.
  flows: []
  scope: address
slug: lifetise-scopes
source_filename: lifetise-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: https://auth.coadjute.com/.well-known/openid-configuration\nraw: well-known/lifetise-openid-configuration.json\nnote: |\n  These are the scopes advertised by Coadjute's Auth0 identity tenant — the standard\n  OpenID Connect scope set plus Auth0's per-claim scopes. They are the real, publicly\n  fetchable scope surface, but they describe identity claims, NOT the authorization\n  model of the Coadjute Network's Partner Cloud API. No Coadjute product/API scopes are\n  published anywhere public: api.coadjute.com answers 401 to every anonymous request and\n  developer.coadjute.com (which once carried an API Catalogue) returns 502. Do not read\n  this list as the network's permission model.\nscope_surface: identity-only\nproduct_scopes_published: false\nschemes:\n- name: coadjute-oidc\n  source: well-known/lifetise-openid-configuration.json\n  issuer: https://auth.coadjute.com/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ https://auth.coadjute.com/authorize\n    tokenUrl: https://auth.coadjute.com/oauth/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://auth.coadjute.com/oauth/token\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://auth.coadjute.com/oauth/device/code\n    tokenUrl: https://auth.coadjute.com/oauth/token\n  - flow: implicit\n    authorizationUrl: https://auth.coadjute.com/authorize\nscopes:\n- scope: openid\n  description: Request an ID token — baseline OpenID Connect authentication.\n  standard: OIDC Core 1.0\n- scope: profile\n  description: Access the end user's default profile claims.\n  standard: OIDC Core 1.0\n- scope: offline_access\n  description: Issue a refresh token for long-lived access.\n  standard: OIDC Core 1.0\n- scope: name\n  description: Access the end user's full name claim.\n- scope: given_name\n  description: Access the end user's given name claim.\n- scope: family_name\n  description: Access the end user's family name claim.\n- scope:\
  \ nickname\n  description: Access the end user's nickname claim.\n- scope: email\n  description: Access the end user's email address claim.\n  standard: OIDC Core 1.0\n- scope: email_verified\n  description: Access whether the end user's email address has been verified.\n- scope: picture\n  description: Access the end user's profile picture claim.\n- scope: created_at\n  description: Access the end user's account creation timestamp (Auth0 claim).\n- scope: identities\n  description: Access the end user's linked identity providers (Auth0 claim).\n- scope: phone\n  description: Access the end user's phone number claim.\n  standard: OIDC Core 1.0\n- scope: address\n  description: Access the end user's address claim.\n  standard: OIDC Core 1.0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lifetise/refs/heads/main/scopes/lifetise-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode/implicit
tags:
- Real Estate
- United Kingdom
- PropTech
- Property Transactions
- Conveyancing
- AML
- Compliance
- Distributed Ledger
- Estate Agents
- Mortgage
token_urls:
- https://auth.coadjute.com/oauth/token
---
