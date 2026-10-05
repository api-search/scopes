---
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Wingtra Scopes
name_suffix: OAuth Scopes
note: 'Wingtra publishes no scope or permission reference — there is no developer portal to publish one on. The scopes below are the `scopes_supported` array the Wingtra Auth0 tenant serves in its own OIDC discovery document, fetched anonymously. They are standard OIDC identity scopes: the tenant advertises no Wingtra product scope (nothing for drones, licences, sites, flights or files), which means the portal GraphQL API and the WingtraCLOUD REST API do not express authorization as OAuth scopes. Authorization is carried instead by tenant membership and by the `assigned_roles` array the login mutation returns, neither of which is documented publicly. scope_count counts what is served, not what governs the API.'
overview: 'Wingtra publishes 14 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Wingtra API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Wingtra
provider_slug: wingtra
schemes: []
scope_count: 14
scope_names:
- openid
- profile
- email
- email_verified
- offline_access
- name
- given_name
- family_name
- nickname
- picture
- phone
- address
- created_at
- identities
scopes:
- description: OIDC — request an ID token.
  flows: []
  scope: openid
- description: OIDC — basic profile claims.
  flows: []
  scope: profile
- description: OIDC — email address.
  flows: []
  scope: email
- description: Whether the email address has been verified.
  flows: []
  scope: email_verified
- description: OIDC — issue a refresh token.
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
- description: Profile picture URL claim.
  flows: []
  scope: picture
- description: Phone number claim.
  flows: []
  scope: phone
- description: Address claim.
  flows: []
  scope: address
- description: Auth0 extension — account creation timestamp.
  flows: []
  scope: created_at
- description: Auth0 extension — linked identity providers for the account.
  flows: []
  scope: identities
slug: wingtra-scopes
source_filename: wingtra-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://my-wingtra.eu.auth0.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Wingtra publishes no scope or permission reference — there is no developer portal to\n  publish one on. The scopes below are the `scopes_supported` array the Wingtra Auth0\n  tenant serves in its own OIDC discovery document, fetched anonymously. They are standard\n  OIDC identity scopes: the tenant advertises no Wingtra product scope (nothing for drones,\n  licences, sites, flights or files), which means the portal GraphQL API and the\n  WingtraCLOUD REST API do not express authorization as OAuth scopes. Authorization is\n  carried instead by tenant membership and by the `assigned_roles` array the login mutation\n  returns, neither of which is documented publicly. scope_count counts what is served, not\n  what governs the API.\nscope_count: 14\nissuer: https://my-wingtra.eu.auth0.com/\nscopes:\n- {name: openid, description: OIDC — request\
  \ an ID token., standard: true}\n- {name: profile, description: OIDC — basic profile claims., standard: true}\n- {name: email, description: OIDC — email address., standard: true}\n- {name: email_verified, description: Whether the email address has been verified., standard: true}\n- {name: offline_access, description: OIDC — issue a refresh token., standard: true}\n- {name: name, description: Full name claim., standard: true}\n- {name: given_name, description: Given name claim., standard: true}\n- {name: family_name, description: Family name claim., standard: true}\n- {name: nickname, description: Nickname claim., standard: true}\n- {name: picture, description: Profile picture URL claim., standard: true}\n- {name: phone, description: Phone number claim., standard: true}\n- {name: address, description: Address claim., standard: true}\n- {name: created_at, description: 'Auth0 extension — account creation timestamp.', standard: false}\n- {name: identities, description: 'Auth0 extension — linked\
  \ identity providers for the account.', standard: false}\nproduct_scopes:\n  count: 0\n  note: >-\n    None. No scope in the tenant names a Wingtra resource, so no API-level scope surface\n    exists to document.\nx-evidence:\n  fetched: '2026-09-04'\n  probes:\n  - {url: 'https://my-wingtra.eu.auth0.com/.well-known/openid-configuration', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wingtra/refs/heads/main/scopes/wingtra-scopes.yml
summary_line: 14 scopes
tags:
- Company
- Drones
- UAV
- Aerial Surveying
- Mapping
- Photogrammetry
- Geospatial
- Surveying
- LiDAR
- Hardware
- Switzerland
token_bound: false
token_urls: []
---
