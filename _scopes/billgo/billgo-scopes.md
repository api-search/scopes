---
authorization_urls:
- https://exchange-login.billgo.com/oauth2/default/v1/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Billgo Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BillGO publishes 8 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BillGO API on a user''s behalf.


  Tokens are issued from https://exchange-login.billgo.com/oauth2/default/v1/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BillGO
provider_slug: billgo
schemes:
- flows:
  - authorizationUrl: https://exchange-login.billgo.com/oauth2/default/v1/authorize
    flow: authorizationCode
    tokenUrl: https://exchange-login.billgo.com/oauth2/default/v1/token
  issuer: https://exchange-login.billgo.com/oauth2/default
  name: BillGO Exchange (Okta default authorization server)
  source: well-known/billgo-openid-configuration.json
scope_count: 8
scope_names:
- interclient_access
- openid
- profile
- email
- address
- phone
- offline_access
- device_sso
scopes:
- description: BillGO-configured scope on the Exchange authorization server; meaning not publicly documented.
  flows:
  - authorizationCode
  scope: interclient_access
- description: Standard OpenID Connect scope requesting an ID token.
  flows: []
  scope: openid
- description: Standard OpenID Connect scope for basic profile claims.
  flows: []
  scope: profile
- description: Standard OpenID Connect scope for the email claim.
  flows: []
  scope: email
- description: Standard OpenID Connect scope for the address claim.
  flows: []
  scope: address
- description: Standard OpenID Connect scope for the phone_number claim.
  flows: []
  scope: phone
- description: Standard OAuth 2.0 scope requesting a refresh token.
  flows: []
  scope: offline_access
- description: Okta device single-sign-on scope.
  flows: []
  scope: device_sso
slug: billgo-scopes
source_filename: billgo-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://exchange-login.billgo.com/oauth2/default/.well-known/openid-configuration\ndocs: null\ndocs_note: >-\n  BillGO publishes no scopes / permissions reference page. docs.billgo.com 302s to a\n  ReadMe login. Every scope below was read out of the provider's own anonymously\n  readable OIDC discovery document — nothing here is inferred or authored.\ncaveat: >-\n  These are the scopes advertised by the Okta \"default\" custom authorization server\n  that fronts BillGO Exchange sign-in, NOT a published BillGO product scope catalogue.\n  All but one are stock OIDC or stock Okta MyAccount scopes that ship with any Okta\n  tenant. `interclient_access` is the only non-stock scope BillGO has configured and\n  exposed on this authorization server; its meaning is not documented publicly.\nschemes:\n- name: BillGO Exchange (Okta default authorization server)\n  source: well-known/billgo-openid-configuration.json\n  issuer: https://exchange-login.billgo.com/oauth2/default\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://exchange-login.billgo.com/oauth2/default/v1/authorize\n    tokenUrl: https://exchange-login.billgo.com/oauth2/default/v1/token\nscopes:\n- scope: interclient_access\n  description: BillGO-configured scope on the Exchange authorization server; meaning not\n    publicly documented.\n  origin: provider-configured\n  flows:\n  - authorizationCode\n  sources:\n  - well-known/billgo-openid-configuration.json\n- scope: openid\n  description: Standard OpenID Connect scope requesting an ID token.\n  origin: standard-oidc\n- scope: profile\n  description: Standard OpenID Connect scope for basic profile claims.\n  origin: standard-oidc\n- scope: email\n  description: Standard OpenID Connect scope for the email claim.\n  origin: standard-oidc\n- scope: address\n  description: Standard OpenID Connect scope for the address claim.\n  origin: standard-oidc\n- scope: phone\n  description: Standard OpenID Connect scope for the phone_number\
  \ claim.\n  origin: standard-oidc\n- scope: offline_access\n  description: Standard OAuth 2.0 scope requesting a refresh token.\n  origin: standard-oauth2\n- scope: device_sso\n  description: Okta device single-sign-on scope.\n  origin: stock-okta\nstock_okta_myaccount_scopes:\n  note: >-\n    Advertised by the same authorization server but supplied by Okta, not BillGO.\n    Listed by name only so the artifact is complete without implying BillGO authored them.\n  scopes:\n  - okta.myAccount.read\n  - okta.myAccount.manage\n  - okta.myAccount.profile.read\n  - okta.myAccount.profile.manage\n  - okta.myAccount.email.read\n  - okta.myAccount.email.manage\n  - okta.myAccount.phone.read\n  - okta.myAccount.phone.manage\n  - okta.myAccount.authenticators.read\n  - okta.myAccount.authenticators.manage\n  - okta.myAccount.appAuthenticator.read\n  - okta.myAccount.appAuthenticator.manage\n  - okta.myAccount.appAuthenticator.maintenance.read\n  - okta.myAccount.appAuthenticator.maintenance.manage\n\
  \  - okta.myAccount.oktaApplications.read\n  - okta.myAccount.organization.read\nx-evidence:\n  fetched: '2026-08-07'\n  probes:\n  - url: https://exchange-login.billgo.com/oauth2/default/.well-known/openid-configuration\n    status: 200\n  - url: https://docs.billgo.com/reference\n    status: 302\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/billgo/refs/heads/main/scopes/billgo-scopes.yml
summary_line: 8 scopes · authorizationCode
tags:
- Payments
- Bill Pay
- Financial Services
- Banking
- ACH
- Virtual Cards
- Fintech
- GraphQL
token_urls:
- https://exchange-login.billgo.com/oauth2/default/v1/token
---
