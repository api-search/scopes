---
authorization_urls: []
description: The scopes below are the verbatim scopes_supported array from the OpenID Connect discovery document Century Communities' own host serves. There is no published scope reference page — the company has no developer portal — so the discovery document is the only authority, and the descriptions are the standard meanings of these identifiers in OpenID Connect and in Optimizely CMS, flagged as such.
docs: ''
flows:
- authorization_code
- client_credentials
- refresh_token
kind: oauth-scopes
layout: scope
method: probed
name: Century Communities Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Century Communities publishes 6 OAuth 2.0 scopes via the authorization_code, client_credentials, and refresh_token flows. Scopes are the fine-grained permissions an application requests at authorization time to act against the Century Communities API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Century Communities
provider_slug: century-communities
schemes: []
scope_count: 6
scope_names:
- openid
- offline_access
- profile
- email
- roles
- epi_service_api
scopes:
- description: Standard OpenID Connect scope requesting an ID token.
  flows: []
  scope: openid
- description: Requests a refresh token so the client can obtain new access tokens without user interaction.
  flows: []
  scope: offline_access
- description: Releases the end user's basic profile claims.
  flows: []
  scope: profile
- description: Releases the end user's email claim.
  flows: []
  scope: email
- description: Releases the end user's role claims; maps to the `role` claim advertised in claims_supported.
  flows: []
  scope: roles
- description: Access to the Optimizely (Episerver) Service API — the authenticated content management surface. Vendor-defined scope, not an OpenID Connect standard scope.
  flows: []
  scope: epi_service_api
slug: century-communities-scopes
source_filename: century-communities-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://www.centurycommunities.com/.well-known/openid-configuration\nprovider: Century Communities\nproviderId: century-communities\ndescription: >-\n  The scopes below are the verbatim scopes_supported array from the OpenID Connect\n  discovery document Century Communities' own host serves. There is no published scope\n  reference page — the company has no developer portal — so the discovery document is the\n  only authority, and the descriptions are the standard meanings of these identifiers in\n  OpenID Connect and in Optimizely CMS, flagged as such.\ndocs: null\ndocs_note: >-\n  No first-party scope/permission reference exists. Searched 2026-09-14; Century\n  Communities publishes no developer documentation.\nissuer: https://www.centurycommunities.com/\nflows:\n  - type: authorization_code\n    pkce: S256\n  - type: client_credentials\n  - type: refresh_token\nscopes:\n  - name: openid\n    description: Standard OpenID Connect\
  \ scope requesting an ID token.\n    standard: OpenID Connect Core 1.0\n  - name: offline_access\n    description: Requests a refresh token so the client can obtain new access tokens without user interaction.\n    standard: OpenID Connect Core 1.0\n  - name: profile\n    description: Releases the end user's basic profile claims.\n    standard: OpenID Connect Core 1.0\n  - name: email\n    description: Releases the end user's email claim.\n    standard: OpenID Connect Core 1.0\n  - name: roles\n    description: Releases the end user's role claims; maps to the `role` claim advertised in claims_supported.\n    standard: Optimizely CMS\n  - name: epi_service_api\n    description: >-\n      Access to the Optimizely (Episerver) Service API — the authenticated content\n      management surface. Vendor-defined scope, not an OpenID Connect standard scope.\n    standard: Optimizely Service API\nscope_count: 6\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/century-communities/refs/heads/main/scopes/century-communities-scopes.yml
summary_line: 6 scopes · authorization_code/client_credentials/refresh_token
tags:
- Real Estate
- Homebuilding
- Construction
- Content Management
- Consumer
- Mortgage
token_bound: false
token_urls: []
---
