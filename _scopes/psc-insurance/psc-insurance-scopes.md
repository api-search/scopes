---
authorization_urls:
- https://login.pscinsurance.com.au/authorize
description: ''
docs: ''
flows:
- authorizationCode
- clientCredentials
- deviceCode
kind: oauth-scopes
layout: scope
method: searched
name: Psc Insurance Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'PSC Insurance publishes 14 OAuth 2.0 scopes via the authorizationCode, clientCredentials, and deviceCode flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the PSC Insurance API on a user''s behalf.


  Tokens are issued from https://login.pscinsurance.com.au/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: PSC Insurance
provider_slug: psc-insurance
schemes:
- flows:
  - authorizationUrl: https://login.pscinsurance.com.au/authorize
    flow: authorizationCode
    tokenUrl: https://login.pscinsurance.com.au/oauth/token
  - flow: clientCredentials
    tokenUrl: https://login.pscinsurance.com.au/oauth/token
  - deviceAuthorizationUrl: https://login.pscinsurance.com.au/oauth/device/code
    flow: deviceCode
    tokenUrl: https://login.pscinsurance.com.au/oauth/token
  name: PSCIdentity
  source: well-known/psc-insurance-openid-configuration.json
scope_count: 14
scope_names:
- openid
- profile
- email
- phone
- address
- offline_access
- name
- given_name
- family_name
- nickname
- email_verified
- picture
- created_at
- identities
scopes:
- description: Request an ID token — the base OpenID Connect scope.
  flows:
  - authorizationCode
  - deviceCode
  scope: openid
- description: Basic profile claims (name, given_name, family_name, nickname, picture).
  flows:
  - authorizationCode
  - deviceCode
  scope: profile
- description: Email address claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: email
- description: Phone number claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: phone
- description: Address claim.
  flows:
  - authorizationCode
  - deviceCode
  scope: address
- description: Issue a refresh token so the session can be renewed without re-auth.
  flows:
  - authorizationCode
  - deviceCode
  scope: offline_access
- description: Auth0 granular profile claim — full name.
  flows: []
  scope: name
- description: Auth0 granular profile claim — given name.
  flows: []
  scope: given_name
- description: Auth0 granular profile claim — family name.
  flows: []
  scope: family_name
- description: Auth0 granular profile claim — nickname.
  flows: []
  scope: nickname
- description: Auth0 granular profile claim — whether the email address is verified.
  flows: []
  scope: email_verified
- description: Auth0 granular profile claim — profile picture URL.
  flows: []
  scope: picture
- description: Auth0 granular profile claim — account creation timestamp.
  flows: []
  scope: created_at
- description: Auth0 granular profile claim — linked identity providers.
  flows: []
  scope: identities
slug: psc-insurance-scopes
source_filename: psc-insurance-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://login.pscinsurance.com.au/.well-known/openid-configuration\ndocs: null\nissuer: https://login.pscinsurance.com.au/\ncaveat: |\n  IMPORTANT — these are NOT documented PSC Insurance API scopes. They are the\n  standard OpenID Connect scopes and Auth0 profile-claim scopes advertised by the\n  tenant discovery document at login.pscinsurance.com.au. PSC publishes no API, no\n  resource server, no audience and no product permission model. This file records\n  the scope surface that is machine-readable and anonymously fetchable, and nothing\n  more. Treat every entry as identity-only.\nschemes:\n- name: PSCIdentity\n  source: well-known/psc-insurance-openid-configuration.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.pscinsurance.com.au/authorize\n    tokenUrl: https://login.pscinsurance.com.au/oauth/token\n  - flow: clientCredentials\n    tokenUrl: https://login.pscinsurance.com.au/oauth/token\n\
  \  - flow: deviceCode\n    deviceAuthorizationUrl: https://login.pscinsurance.com.au/oauth/device/code\n    tokenUrl: https://login.pscinsurance.com.au/oauth/token\nscopes:\n- scope: openid\n  description: Request an ID token — the base OpenID Connect scope.\n  kind: oidc-standard\n  flows: [authorizationCode, deviceCode]\n- scope: profile\n  description: Basic profile claims (name, given_name, family_name, nickname, picture).\n  kind: oidc-standard\n  flows: [authorizationCode, deviceCode]\n- scope: email\n  description: Email address claim.\n  kind: oidc-standard\n  flows: [authorizationCode, deviceCode]\n- scope: phone\n  description: Phone number claim.\n  kind: oidc-standard\n  flows: [authorizationCode, deviceCode]\n- scope: address\n  description: Address claim.\n  kind: oidc-standard\n  flows: [authorizationCode, deviceCode]\n- scope: offline_access\n  description: Issue a refresh token so the session can be renewed without re-auth.\n  kind: oidc-standard\n  flows: [authorizationCode,\
  \ deviceCode]\n- scope: name\n  description: Auth0 granular profile claim — full name.\n  kind: auth0-profile-claim\n- scope: given_name\n  description: Auth0 granular profile claim — given name.\n  kind: auth0-profile-claim\n- scope: family_name\n  description: Auth0 granular profile claim — family name.\n  kind: auth0-profile-claim\n- scope: nickname\n  description: Auth0 granular profile claim — nickname.\n  kind: auth0-profile-claim\n- scope: email_verified\n  description: Auth0 granular profile claim — whether the email address is verified.\n  kind: auth0-profile-claim\n- scope: picture\n  description: Auth0 granular profile claim — profile picture URL.\n  kind: auth0-profile-claim\n- scope: created_at\n  description: Auth0 granular profile claim — account creation timestamp.\n  kind: auth0-profile-claim\n- scope: identities\n  description: Auth0 granular profile claim — linked identity providers.\n  kind: auth0-profile-claim\nproduct_scopes:\n  documented: false\n  note: |\n    No\
  \ PSC-specific scope (policy:read, claim:write, quote:create or anything of that\n    shape) is documented or advertised. If broker/client portal APIs exist behind this\n    tenant they are private and their audiences are not published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/psc-insurance/refs/heads/main/scopes/psc-insurance-scopes.yml
summary_line: 14 scopes · authorizationCode/clientCredentials/deviceCode
tags:
- Insurance
- Australia
- Brokers
- Insurance Brokerage
- Property and Casualty
- Commercial Insurance
- Cyber Insurance
- Intermediary
- Partner Gated
- No Public API
token_urls:
- https://login.pscinsurance.com.au/oauth/token
---
