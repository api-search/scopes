---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Aig Scopes
name_suffix: OAuth Scopes
note: Read from AIG's own anonymously-served OAuth 2.0 / OpenID Connect discovery documents. AIG publishes no scopes reference page, so descriptions below are the standard OIDC/Okta meanings for the standard scopes and are left null for the two AIG-specific scopes rather than guessed.
overview: 'AIG uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: AIG
provider_slug: aig
schemes:
- issuer: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7
  name: AIG Customer Platform authorization server
  scopes:
  - description: null
    name: emeasme
    note: AIG-specific scope; no published definition. Name suggests the EMEA SME book of business.
  - description: null
    name: interclient_access
    note: AIG-specific scope; no published definition.
  - description: Request an ID token (OpenID Connect).
    name: openid
  - description: Standard OIDC profile claims.
    name: profile
  - description: Standard OIDC email claims.
    name: email
  - description: Standard OIDC address claim.
    name: address
  - description: Standard OIDC phone claims.
    name: phone
  - description: Issue a refresh token.
    name: offline_access
  - description: Okta device single sign-on.
    name: device_sso
  - description: Okta platform scope — read the end user's app authenticator enrollment.
    name: okta.myAccount.appAuthenticator.read
  - description: Okta platform scope — manage the end user's app authenticator enrollment.
    name: okta.myAccount.appAuthenticator.manage
  - description: Okta platform scope — read app authenticator maintenance state.
    name: okta.myAccount.appAuthenticator.maintenance.read
  - description: Okta platform scope — manage app authenticator maintenance state.
    name: okta.myAccount.appAuthenticator.maintenance.manage
  source: well-known/aig-oauth-authorization-server.json
- issuer: https://auth1.customerpltfm.aig.com
  name: AIG Okta org issuer
  scopes:
  - description: Request an ID token (OpenID Connect).
    name: openid
  - description: Standard OIDC email claims.
    name: email
  - description: Standard OIDC profile claims.
    name: profile
  - description: Standard OIDC address claim.
    name: address
  - description: Standard OIDC phone claims.
    name: phone
  - description: Issue a refresh token.
    name: offline_access
  - description: Group memberships of the authenticated user.
    name: groups
  source: well-known/aig-openid-configuration.json
scope_count: 0
scope_names: []
scopes: []
slug: aig-scopes
source_filename: aig-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/.well-known/oauth-authorization-server\n  (HTTP 200) and https://auth1.customerpltfm.aig.com/.well-known/openid-configuration (HTTP 200)\nnote: >-\n  Read from AIG's own anonymously-served OAuth 2.0 / OpenID Connect discovery documents. AIG\n  publishes no scopes reference page, so descriptions below are the standard OIDC/Okta meanings\n  for the standard scopes and are left null for the two AIG-specific scopes rather than guessed.\ndocs: null\nschemes:\n  - name: AIG Customer Platform authorization server\n    issuer: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7\n    source: well-known/aig-oauth-authorization-server.json\n    scopes:\n      - name: emeasme\n        description: null\n        note: AIG-specific scope; no published definition. Name suggests the EMEA SME book of business.\n      - name: interclient_access\n        description:\
  \ null\n        note: AIG-specific scope; no published definition.\n      - name: openid\n        description: Request an ID token (OpenID Connect).\n      - name: profile\n        description: Standard OIDC profile claims.\n      - name: email\n        description: Standard OIDC email claims.\n      - name: address\n        description: Standard OIDC address claim.\n      - name: phone\n        description: Standard OIDC phone claims.\n      - name: offline_access\n        description: Issue a refresh token.\n      - name: device_sso\n        description: Okta device single sign-on.\n      - name: okta.myAccount.appAuthenticator.read\n        description: Okta platform scope — read the end user's app authenticator enrollment.\n      - name: okta.myAccount.appAuthenticator.manage\n        description: Okta platform scope — manage the end user's app authenticator enrollment.\n      - name: okta.myAccount.appAuthenticator.maintenance.read\n        description: Okta platform scope — read\
  \ app authenticator maintenance state.\n      - name: okta.myAccount.appAuthenticator.maintenance.manage\n        description: Okta platform scope — manage app authenticator maintenance state.\n  - name: AIG Okta org issuer\n    issuer: https://auth1.customerpltfm.aig.com\n    source: well-known/aig-openid-configuration.json\n    scopes:\n      - name: openid\n        description: Request an ID token (OpenID Connect).\n      - name: email\n        description: Standard OIDC email claims.\n      - name: profile\n        description: Standard OIDC profile claims.\n      - name: address\n        description: Standard OIDC address claim.\n      - name: phone\n        description: Standard OIDC phone claims.\n      - name: offline_access\n        description: Issue a refresh token.\n      - name: groups\n        description: Group memberships of the authenticated user.\nscope_count: 20\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aig/refs/heads/main/scopes/aig-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Insurance
- Financial-Services
- Property Casualty
- Cyber Insurance
- Enterprise
- Fortune 100
token_urls: []
---
