---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: World Fuel Services Scopes
name_suffix: OAuth Scopes
note: 'These are the values in `scopes_supported` on World Kinect''s own OIDC discovery document, copied verbatim. There is no published scopes/permissions reference page, and no API-specific (audience) scopes are advertised anonymously — the list is the standard OpenID Connect / Auth0 profile set, which tells an integrator what identity claims the portal''s tokens can carry but nothing about what the underlying fuel, pricing or trip APIs authorize. derive-oauth-scopes.py was not run: it derives from OpenAPI oauth2 securitySchemes and this provider publishes no OpenAPI.'
overview: 'World Fuel Services publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the World Fuel Services API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: World Fuel Services
provider_slug: world-fuel-services
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
- description: OpenID Connect — request an ID token.
  flows: []
  scope: openid
- description: Standard profile claims.
  flows: []
  scope: profile
- description: Issue a refresh token.
  flows: []
  scope: offline_access
- description: name claim.
  flows: []
  scope: name
- description: given_name claim.
  flows: []
  scope: given_name
- description: family_name claim.
  flows: []
  scope: family_name
- description: nickname claim.
  flows: []
  scope: nickname
- description: email claim.
  flows: []
  scope: email
- description: email_verified claim.
  flows: []
  scope: email_verified
- description: picture claim.
  flows: []
  scope: picture
- description: created_at claim.
  flows: []
  scope: created_at
- description: Linked identity providers for the user.
  flows: []
  scope: identities
- description: phone_number claim.
  flows: []
  scope: phone
- description: address claim.
  flows: []
  scope: address
slug: world-fuel-services-scopes
source_filename: world-fuel-services-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://auth.wfscorp.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  These are the values in `scopes_supported` on World Kinect's own OIDC discovery document,\n  copied verbatim. There is no published scopes/permissions reference page, and no\n  API-specific (audience) scopes are advertised anonymously — the list is the standard OpenID\n  Connect / Auth0 profile set, which tells an integrator what identity claims the portal's\n  tokens can carry but nothing about what the underlying fuel, pricing or trip APIs authorize.\n  derive-oauth-scopes.py was not run: it derives from OpenAPI oauth2 securitySchemes and this\n  provider publishes no OpenAPI.\nauthorization_server: https://auth.wfscorp.com/\nscope_count: 14\nscopes:\n- scope: openid\n  description: OpenID Connect — request an ID token.\n- scope: profile\n  description: Standard profile claims.\n- scope: offline_access\n  description: Issue a refresh token.\n\
  - scope: name\n  description: name claim.\n- scope: given_name\n  description: given_name claim.\n- scope: family_name\n  description: family_name claim.\n- scope: nickname\n  description: nickname claim.\n- scope: email\n  description: email claim.\n- scope: email_verified\n  description: email_verified claim.\n- scope: picture\n  description: picture claim.\n- scope: created_at\n  description: created_at claim.\n- scope: identities\n  description: Linked identity providers for the user.\n- scope: phone\n  description: phone_number claim.\n- scope: address\n  description: address claim.\nclaims_supported:\n- aud\n- auth_time\n- created_at\n- email\n- email_verified\n- exp\n- family_name\n- given_name\n- iat\n- identities\n- iss\n- name\n- nickname\n- phone_number\n- picture\n- sub\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/world-fuel-services/refs/heads/main/scopes/world-fuel-services-scopes.yml
summary_line: 14 scopes
tags:
- Fortune 100
- Energy
- Aviation Fuel
- Marine Fuel
- Fuel Distribution
- Energy Management
- Sustainability
- Logistics
- Fuel Cards
token_urls: []
---
