---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Swift Navigation Scopes
name_suffix: OAuth Scopes
note: The derive-oauth-scopes.py baseline could not run — it reads oauth2 securitySchemes from an OpenAPI and Swift Navigation publishes none. These scopes are read directly from the discovery document of the Auth0 tenant that fronts the Skylark User Portal and its backend services, identified from https://account.swiftnav.com/runtime-config.js.
overview: 'Swift Navigation publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Swift Navigation API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Swift Navigation
provider_slug: swift-navigation
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
- description: Issue an ID token (OIDC core).
  flows: []
  scope: openid
- description: Basic profile claims.
  flows: []
  scope: profile
- description: Issue a refresh token.
  flows: []
  scope: offline_access
- description: Full name claim.
  flows: []
  scope: name
- description: Given name claim.
  flows: []
  scope: given_name
- description: Family name claim.
  flows: []
  scope: family_name
- description: Nickname claim.
  flows: []
  scope: nickname
- description: Email address claim.
  flows: []
  scope: email
- description: Email verification status claim.
  flows: []
  scope: email_verified
- description: Profile picture claim.
  flows: []
  scope: picture
- description: Account creation timestamp claim.
  flows: []
  scope: created_at
- description: Linked identity providers claim.
  flows: []
  scope: identities
- description: Phone number claim.
  flows: []
  scope: phone
- description: Address claim.
  flows: []
  scope: address
slug: swift-navigation-scopes
source_filename: swift-navigation-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://skylark-prod.us.auth0.com/.well-known/openid-configuration (HTTP 200, 2026-08-29)\nname: Swift Navigation OAuth scopes\nnote: >-\n  The derive-oauth-scopes.py baseline could not run — it reads oauth2 securitySchemes from an OpenAPI\n  and Swift Navigation publishes none. These scopes are read directly from the discovery document of\n  the Auth0 tenant that fronts the Skylark User Portal and its backend services, identified from\n  https://account.swiftnav.com/runtime-config.js.\ndocs: null\ndocs_note: >-\n  No scopes or permissions reference page is published. Searched support.swiftnav.com (152-URL\n  sitemap) and www.swiftnav.com — neither documents an authorization model.\nissuer: https://skylark-prod.us.auth0.com/\naudience: https://account.swiftnav.com\nfinding: >-\n  Every advertised scope is a stock OIDC identity scope. There is NOT ONE Skylark-specific API scope\n  — no read:devices, no write:subscriptions, no\
  \ manage:credentials. A token issued by this tenant\n  carries identity claims and nothing that describes what it may do to a Skylark account, which means\n  an integrator (or an agent) cannot reason about least privilege before requesting one, and cannot\n  scope a token down if they wanted to.\nscopes:\n  - {name: openid, description: 'Issue an ID token (OIDC core).'}\n  - {name: profile, description: 'Basic profile claims.'}\n  - {name: offline_access, description: 'Issue a refresh token.'}\n  - {name: name, description: Full name claim.}\n  - {name: given_name, description: Given name claim.}\n  - {name: family_name, description: Family name claim.}\n  - {name: nickname, description: Nickname claim.}\n  - {name: email, description: Email address claim.}\n  - {name: email_verified, description: Email verification status claim.}\n  - {name: picture, description: Profile picture claim.}\n  - {name: created_at, description: Account creation timestamp claim.}\n  - {name: identities, description:\
  \ Linked identity providers claim.}\n  - {name: phone, description: Phone number claim.}\n  - {name: address, description: Address claim.}\ngrant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - implicit\n  - password\n  - 'urn:ietf:params:oauth:grant-type:device_code'\n  - 'urn:ietf:params:oauth:grant-type:token-exchange'\n  - 'urn:ietf:params:oauth:grant-type:jwt-bearer'\npkce: [S256, plain]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swift-navigation/refs/heads/main/scopes/swift-navigation-scopes.yml
summary_line: 14 scopes
tags:
- Company
- GNSS
- Precise Positioning
- Location
- Corrections
- RTK
- NTRIP
- RTCM
- Automotive
- Geospatial
- IoT
- Robotics
- Protocol
token_bound: false
token_urls: []
---
