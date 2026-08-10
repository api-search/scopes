---
authorization_urls:
- https://sso.place.com/oauth2/v1/authorize
- https://sso.place.com/oauth2/default/v1/authorize
- https://hub.place.com/oauth2/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Place Scopes
name_suffix: OAuth Scopes
note: These scopes come from the scopes_supported arrays of the OAuth 2.0 / OpenID Connect discovery documents PLACE serves from sso.place.com and hub.place.com. PLACE publishes no scopes reference page and no product API, so no PLACE-authored product scopes exist. The okta.* set is the Okta Org Authorization Server management scope catalog shipped by the identity vendor — it is recorded for fidelity and is explicitly NOT a PLACE product scope surface.
overview: 'PLACE publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the PLACE API on a user''s behalf.


  Tokens are issued from https://sso.place.com/oauth2/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PLACE
provider_slug: place
schemes:
- flows:
  - authorizationUrl: https://sso.place.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://sso.place.com/oauth2/v1/token
  issuer: https://sso.place.com
  name: PLACE SSO
  source: well-known/place-sso-openid-configuration.json
- flows:
  - authorizationUrl: https://sso.place.com/oauth2/default/v1/authorize
    flow: authorizationCode
    tokenUrl: https://sso.place.com/oauth2/default/v1/token
  issuer: https://sso.place.com/oauth2/default
  name: PLACE SSO default authorization server
  source: well-known/place-sso-default-openid-configuration.json
- flows:
  - authorizationUrl: https://hub.place.com/oauth2/v1/authorize
    flow: authorizationCode
    tokenUrl: https://hub.place.com/oauth2/v1/token
  issuer: https://hub.place.com
  name: PLACE identity hub
  source: well-known/place-hub-openid-configuration.json
scope_count: 8
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- groups
- device_sso
scopes:
- description: OpenID Connect authentication; returns an ID token.
  flows: []
  scope: openid
- description: Basic profile claims (name, family_name, given_name, locale, zoneinfo).
  flows: []
  scope: profile
- description: email and email_verified claims.
  flows: []
  scope: email
- description: address claim.
  flows: []
  scope: address
- description: phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Issues a refresh token for long-lived access.
  flows: []
  scope: offline_access
- description: Group membership claim.
  flows: []
  scope: groups
- description: Device single-sign-on token exchange.
  flows: []
  scope: device_sso
slug: place-scopes
source_filename: place-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: well-known/place-sso-openid-configuration.json, well-known/place-sso-default-openid-configuration.json,\n  well-known/place-hub-openid-configuration.json, well-known/place-sso-oauth-authorization-server.json\ndocs: null\nnote: >-\n  These scopes come from the scopes_supported arrays of the OAuth 2.0 / OpenID Connect\n  discovery documents PLACE serves from sso.place.com and hub.place.com. PLACE publishes\n  no scopes reference page and no product API, so no PLACE-authored product scopes exist.\n  The okta.* set is the Okta Org Authorization Server management scope catalog shipped by\n  the identity vendor — it is recorded for fidelity and is explicitly NOT a PLACE product\n  scope surface.\nschemes:\n- name: PLACE SSO\n  issuer: https://sso.place.com\n  source: well-known/place-sso-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sso.place.com/oauth2/v1/authorize\n    tokenUrl: https://sso.place.com/oauth2/v1/token\n\
  - name: PLACE SSO default authorization server\n  issuer: https://sso.place.com/oauth2/default\n  source: well-known/place-sso-default-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sso.place.com/oauth2/default/v1/authorize\n    tokenUrl: https://sso.place.com/oauth2/default/v1/token\n- name: PLACE identity hub\n  issuer: https://hub.place.com\n  source: well-known/place-hub-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://hub.place.com/oauth2/v1/authorize\n    tokenUrl: https://hub.place.com/oauth2/v1/token\nscopes:\n- scope: openid\n  description: OpenID Connect authentication; returns an ID token.\n  standard: OpenID Connect Core 1.0\n  issuers: [https://sso.place.com, 'https://sso.place.com/oauth2/default', https://hub.place.com]\n- scope: profile\n  description: Basic profile claims (name, family_name, given_name, locale, zoneinfo).\n  standard: OpenID Connect Core 1.0\n  issuers: [https://sso.place.com,\
  \ 'https://sso.place.com/oauth2/default', https://hub.place.com]\n- scope: email\n  description: email and email_verified claims.\n  standard: OpenID Connect Core 1.0\n  issuers: [https://sso.place.com, 'https://sso.place.com/oauth2/default', https://hub.place.com]\n- scope: address\n  description: address claim.\n  standard: OpenID Connect Core 1.0\n  issuers: [https://sso.place.com, 'https://sso.place.com/oauth2/default', https://hub.place.com]\n- scope: phone\n  description: phone_number and phone_number_verified claims.\n  standard: OpenID Connect Core 1.0\n  issuers: [https://sso.place.com, 'https://sso.place.com/oauth2/default', https://hub.place.com]\n- scope: offline_access\n  description: Issues a refresh token for long-lived access.\n  standard: OpenID Connect Core 1.0\n  issuers: [https://sso.place.com, 'https://sso.place.com/oauth2/default', https://hub.place.com]\n- scope: groups\n  description: Group membership claim.\n  standard: Okta extension\n  issuers: [https://sso.place.com,\
  \ 'https://sso.place.com/oauth2/default', https://hub.place.com]\n- scope: device_sso\n  description: Device single-sign-on token exchange.\n  standard: Okta extension\n  issuers: ['https://sso.place.com/oauth2/default']\nvendor_scopes:\n  vendor: Okta\n  prefix: 'okta.'\n  count: 80\n  authored_by_place: false\n  sources:\n  - well-known/place-sso-oauth-authorization-server.json\n  - well-known/place-hub-oauth-authorization-server.json\n  description: >-\n    Okta Org Authorization Server management scopes (okta.users.*, okta.groups.*,\n    okta.apps.*, okta.policies.*, okta.logs.read, …). They govern administration of\n    PLACE's Okta tenant, not any PLACE product API, and are shipped identically by\n    every Okta org.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/place/refs/heads/main/scopes/place-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Company
- Real Estate
- Property Technology
- PropTech
- CRM
- Transaction Management
- Brokerage
- MLS
- Mortgage
- Title and Escrow
- Business Services
- Identity
token_urls:
- https://sso.place.com/oauth2/v1/token
- https://sso.place.com/oauth2/default/v1/token
- https://hub.place.com/oauth2/v1/token
---
