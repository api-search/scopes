---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: American International Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'American International Group (AIG) publishes 13 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the American International Group (AIG) API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: American International Group (AIG)
provider_slug: american-international
schemes: []
scope_count: 13
scope_names:
- openid
- profile
- email
- address
- phone
- offline_access
- device_sso
- interclient_access
- emeasme
- okta.myAccount.appAuthenticator.manage
- okta.myAccount.appAuthenticator.read
- okta.myAccount.appAuthenticator.maintenance.manage
- okta.myAccount.appAuthenticator.maintenance.read
scopes:
- description: OpenID Connect authentication; required to receive an ID token.
  flows: []
  scope: openid
- description: Basic profile claims (name, preferred_username, locale, updated_at).
  flows: []
  scope: profile
- description: The email and email_verified claims.
  flows: []
  scope: email
- description: The address claim.
  flows: []
  scope: address
- description: The phone_number and phone_number_verified claims.
  flows: []
  scope: phone
- description: Issues a refresh token so the client can renew access without user interaction.
  flows: []
  scope: offline_access
- description: Okta device single-sign-on; binds the token to a registered device.
  flows: []
  scope: device_sso
- description: Okta token-exchange scope permitting one client's token to be exchanged for another client's. AIG-configured; no AIG documentation states which clients it bridges.
  flows: []
  scope: interclient_access
- description: AIG-specific custom scope. The name reads as EMEA + SME (small and medium enterprise), which would match AIG's EMEA small-business lines, but AIG publishes nothing that states its meaning or the resources it grants. Recorded as UNKNOWN — the reading is an observation, not a claim.
  flows: []
  scope: emeasme
- description: Manage the user's own Okta app authenticator enrollment.
  flows: []
  scope: okta.myAccount.appAuthenticator.manage
- description: Read the user's own Okta app authenticator enrollment.
  flows: []
  scope: okta.myAccount.appAuthenticator.read
- description: Manage maintenance state of the user's own Okta app authenticator.
  flows: []
  scope: okta.myAccount.appAuthenticator.maintenance.manage
- description: Read maintenance state of the user's own Okta app authenticator.
  flows: []
  scope: okta.myAccount.appAuthenticator.maintenance.read
slug: american-international-scopes
source_filename: american-international-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7/.well-known/oauth-authorization-server\n  (HTTP 200, fetched anonymously 2026-09-02)\nprovider: American International Group (AIG)\nproviderId: american-international\ndocs: null\ndocs_note: >-\n  AIG publishes no scopes or permissions reference page. Every scope below is read verbatim from\n  the scopes_supported array of AIG's own anonymously-served authorization-server metadata; the\n  descriptions are the standard OIDC/Okta meanings, and the two AIG-specific scopes are recorded\n  with their meaning marked unknown rather than guessed.\nauthorization_server: https://auth1.customerpltfm.aig.com/oauth2/aus1aaqj1zvwVDL2n5d7\nscope_count: 13\nscopes:\n  - name: openid\n    description: OpenID Connect authentication; required to receive an ID token.\n    standard: true\n  - name: profile\n    description: Basic profile claims (name, preferred_username, locale,\
  \ updated_at).\n    standard: true\n  - name: email\n    description: The email and email_verified claims.\n    standard: true\n  - name: address\n    description: The address claim.\n    standard: true\n  - name: phone\n    description: The phone_number and phone_number_verified claims.\n    standard: true\n  - name: offline_access\n    description: Issues a refresh token so the client can renew access without user interaction.\n    standard: true\n  - name: device_sso\n    description: Okta device single-sign-on; binds the token to a registered device.\n    standard: false\n    vendor: Okta\n  - name: interclient_access\n    description: >-\n      Okta token-exchange scope permitting one client's token to be exchanged for another client's.\n      AIG-configured; no AIG documentation states which clients it bridges.\n    standard: false\n    vendor: Okta\n  - name: emeasme\n    description: >-\n      AIG-specific custom scope. The name reads as EMEA + SME (small and medium enterprise),\
  \ which\n      would match AIG's EMEA small-business lines, but AIG publishes nothing that states its meaning\n      or the resources it grants. Recorded as UNKNOWN — the reading is an observation, not a claim.\n    standard: false\n    vendor: AIG\n    meaning: unknown\n  - name: okta.myAccount.appAuthenticator.manage\n    description: Manage the user's own Okta app authenticator enrollment.\n    standard: false\n    vendor: Okta\n  - name: okta.myAccount.appAuthenticator.read\n    description: Read the user's own Okta app authenticator enrollment.\n    standard: false\n    vendor: Okta\n  - name: okta.myAccount.appAuthenticator.maintenance.manage\n    description: Manage maintenance state of the user's own Okta app authenticator.\n    standard: false\n    vendor: Okta\n  - name: okta.myAccount.appAuthenticator.maintenance.read\n    description: Read maintenance state of the user's own Okta app authenticator.\n    standard: false\n    vendor: Okta\nfinding: >-\n  Of the 13 scopes AIG's\
  \ customer-platform authorization server advertises, 11 are stock OIDC or\n  Okta platform scopes and exactly ONE (emeasme) is an AIG business scope. There is no scope that\n  names an insurance resource — no policy, quote, claim, certificate or producer scope is exposed\n  anonymously. Whatever authorization the commercial gateway applies is not expressed in the\n  discoverable scope set.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-international/refs/heads/main/scopes/american-international-scopes.yml
summary_line: 13 scopes
tags:
- Insurance
- Property Casualty
- Cyber Insurance
- Commercial Insurance
- Global Insurance
- Financial Services
- Reinsurance
- Fortune 500
token_bound: false
token_urls: []
---
