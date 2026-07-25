---
authorization_urls:
- https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/authorize
- https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Bupa Australia Scopes
name_suffix: OAuth Scopes
note: Bupa Australia publishes NO API scopes. The scopes below are the OpenID Connect scopes advertised by the two sign-in surfaces — they authorize a human session against the partner portal and the developer portal, not a machine-to-machine call against a Bupa API. The API gateway (api.bupa.com.au) returns 502 anonymously and the developer portal releases API specifications only after contact with the Bupa Integration Fabric Team, so any per-API scope or permission model remains unpublished. Recording the identity scopes is the honest floor, not a claim of an API scope surface.
overview: 'Bupa Australia publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Bupa Australia API on a user''s behalf.


  Tokens are issued from https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Bupa Australia
provider_slug: bupa-australia
schemes:
- flows:
  - authorizationUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/token
  guards: https://partner.bupa.com.au/
  name: partner-portal-b2c
  source: well-known/bupa-australia-partner-b2c-openid-configuration.json
- flows:
  - authorizationUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/authorize
    flow: authorizationCode
    tokenUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/token
  guards: https://portal.api.bupa.com.au/signin
  name: developer-portal-entra
  source: well-known/bupa-australia-portal-entra-openid-configuration.json
scope_count: 4
scope_names:
- openid
- profile
- email
- offline_access
scopes:
- description: OpenID Connect sign-in; issues an RS256 id_token with a pairwise subject.
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile claims on the developer-portal Entra sign-in.
  flows:
  - authorizationCode
  scope: profile
- description: Email claim on the developer-portal Entra sign-in.
  flows:
  - authorizationCode
  scope: email
- description: Refresh-token issuance on the developer-portal Entra sign-in.
  flows:
  - authorizationCode
  scope: offline_access
slug: bupa-australia-scopes
source_filename: bupa-australia-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: |\n  The two anonymously readable OpenID Connect discovery documents saved in\n  well-known/, fetched 2026-07-25. There is no OpenAPI for this provider, so no\n  scope could be derived from a spec.\nscope: identity-only\nnote: |\n  Bupa Australia publishes NO API scopes. The scopes below are the OpenID\n  Connect scopes advertised by the two sign-in surfaces — they authorize a\n  human session against the partner portal and the developer portal, not a\n  machine-to-machine call against a Bupa API. The API gateway\n  (api.bupa.com.au) returns 502 anonymously and the developer portal releases\n  API specifications only after contact with the Bupa Integration Fabric Team,\n  so any per-API scope or permission model remains unpublished. Recording the\n  identity scopes is the honest floor, not a claim of an API scope surface.\nschemes:\n- name: partner-portal-b2c\n  source: well-known/bupa-australia-partner-b2c-openid-configuration.json\n\
  \  guards: https://partner.bupa.com.au/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/authorize\n    tokenUrl: https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/token\n- name: developer-portal-entra\n  source: well-known/bupa-australia-portal-entra-openid-configuration.json\n  guards: https://portal.api.bupa.com.au/signin\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/token\nscopes:\n- scope: openid\n  description: OpenID Connect sign-in; issues an RS256 id_token with a pairwise subject.\n  kind: identity\n  flows: [authorizationCode]\n  sources:\n  - well-known/bupa-australia-partner-b2c-openid-configuration.json\n\
  \  - well-known/bupa-australia-portal-entra-openid-configuration.json\n- scope: profile\n  description: Basic profile claims on the developer-portal Entra sign-in.\n  kind: identity\n  flows: [authorizationCode]\n  sources: [well-known/bupa-australia-portal-entra-openid-configuration.json]\n- scope: email\n  description: Email claim on the developer-portal Entra sign-in.\n  kind: identity\n  flows: [authorizationCode]\n  sources: [well-known/bupa-australia-portal-entra-openid-configuration.json]\n- scope: offline_access\n  description: Refresh-token issuance on the developer-portal Entra sign-in.\n  kind: identity\n  flows: [authorizationCode]\n  sources: [well-known/bupa-australia-portal-entra-openid-configuration.json]\napi_scopes: []\napi_scopes_note: |\n  None published. The B2C discovery document advertises scopes_supported\n  [\"openid\"] and nothing else; no resource scope, no application ID URI and no\n  audience for any Bupa API appears on any anonymously reachable surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bupa-australia/refs/heads/main/scopes/bupa-australia-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Insurance
- Australia
- Health Insurance
- Private Health Insurance
- Carrier
- Healthcare
- Claims
- Policy Administration
- Employee Benefits
- Partner Gated
token_urls:
- https://partnerlogin.bupa.com.au/52bddae3-95ef-41bb-8c87-5561dead0bad/b2c_1a_prod_01_signup_signin/oauth2/v2.0/token
- https://login.microsoftonline.com/fee9c112-179f-46e3-ab98-f8d58602cf19/oauth2/v2.0/token
---
