---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Polaris Industries Scopes
name_suffix: OAuth Scopes
note: 'These are the scopes_supported advertised by the OpenID Connect discovery document for the Polaris dealer-portal identity tenant. They are standard OIDC/Auth0 identity scopes — there are NO Polaris business/API scopes published anywhere, because Polaris publishes no public API. Do not read this file as an API permission model; it is the identity surface only. The live dealer-portal login requests only: openid profile email offline_access.'
overview: 'Polaris Industries publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Polaris Industries API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Polaris Industries
provider_slug: polaris-industries
schemes: []
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
- description: OIDC — request an ID token.
  flows: []
  scope: openid
- description: OIDC — basic profile claims.
  flows: []
  scope: profile
- description: OIDC — issue a refresh token.
  flows: []
  scope: offline_access
- description: Identity claim — full name.
  flows: []
  scope: name
- description: Identity claim — given name.
  flows: []
  scope: given_name
- description: Identity claim — family name.
  flows: []
  scope: family_name
- description: Identity claim — nickname.
  flows: []
  scope: nickname
- description: Identity claim — email address.
  flows: []
  scope: email
- description: Identity claim — whether the email address is verified.
  flows: []
  scope: email_verified
- description: Identity claim — profile picture URL.
  flows: []
  scope: picture
- description: Identity claim — account creation timestamp.
  flows: []
  scope: created_at
- description: Identity claim — linked identity providers.
  flows: []
  scope: identities
- description: Identity claim — phone number.
  flows: []
  scope: phone
- description: Identity claim — postal address.
  flows: []
  scope: address
slug: polaris-industries-scopes
source_filename: polaris-industries-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: https://polarisdealers.auth0.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  These are the scopes_supported advertised by the OpenID Connect discovery document for the\n  Polaris dealer-portal identity tenant. They are standard OIDC/Auth0 identity scopes — there\n  are NO Polaris business/API scopes published anywhere, because Polaris publishes no public\n  API. Do not read this file as an API permission model; it is the identity surface only.\n  The live dealer-portal login requests only: openid profile email offline_access.\nissuer: https://polarisdealers.auth0.com/\naudience: https://polarisportal.com\nrequested_by_dealer_portal:\n- openid\n- profile\n- email\n- offline_access\nscopes:\n- name: openid\n  description: OIDC — request an ID token.\n- name: profile\n  description: OIDC — basic profile claims.\n- name: offline_access\n  description: OIDC — issue a refresh token.\n- name: name\n  description: Identity\
  \ claim — full name.\n- name: given_name\n  description: Identity claim — given name.\n- name: family_name\n  description: Identity claim — family name.\n- name: nickname\n  description: Identity claim — nickname.\n- name: email\n  description: Identity claim — email address.\n- name: email_verified\n  description: Identity claim — whether the email address is verified.\n- name: picture\n  description: Identity claim — profile picture URL.\n- name: created_at\n  description: Identity claim — account creation timestamp.\n- name: identities\n  description: Identity claim — linked identity providers.\n- name: phone\n  description: Identity claim — phone number.\n- name: address\n  description: Identity claim — postal address.\nclaims_supported:\n- aud\n- auth_time\n- created_at\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- identities\n- iss\n- name\n- nickname\n- phone_number\n- picture\n- sub\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polaris-industries/refs/heads/main/scopes/polaris-industries-scopes.yml
summary_line: 14 scopes
tags:
- Fortune 1000
- Manufacturing
- Power-Sports
- Automotive
- Consumer Products
- Connected Vehicles
- Marine
token_bound: false
token_urls: []
---
