---
api_specs:
- filename: gadjah-mada-university-ugm-id-openapi.yml
  format: yaml
  label: UGM ID — OAuth 2.0 / OpenID Connect Authorization Server
  slug: ugm-id
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-ugm-id-openapi.yml
- filename: gadjah-mada-university-repository-oai-pmh-openapi.yml
  format: yaml
  label: UGM Institutional Repository OAI-PMH
  slug: repository-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-repository-oai-pmh-openapi.yml
- filename: gadjah-mada-university-journal-oai-pmh-openapi.yml
  format: yaml
  label: UGM Journals OAI-PMH
  slug: journal-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/openapi/gadjah-mada-university-journal-oai-pmh-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Gadjah Mada University Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Gadjah Mada University publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Gadjah Mada University API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Gadjah Mada University
provider_slug: gadjah-mada-university
schemes: []
scope_count: 5
scope_names:
- openid
- profile
- email
- user.read
- userDetail.read
scopes:
- description: Requests an id_token and enables the OIDC UserInfo endpoint.
  flows: []
  scope: openid
- description: Basic profile claims - name, given_name, family_name, picture, preferred_username, plus UGM's non-standard unit_id claim.
  flows: []
  scope: profile
- description: Email claims.
  flows: []
  scope: email
- description: Read the authenticated subject's basic user profile.
  flows: []
  scope: user.read
- description: Read the full Simaster user record, and read another user's record by username. The broadest scope the server issues.
  flows: []
  scope: userDetail.read
slug: gadjah-mada-university-scopes
source_filename: gadjah-mada-university-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\ngenerated: '2026-09-01'\nmethod: searched\nsource: >-\n  Read verbatim on 2026-09-01 from UGM's own published discovery documents at\n  https://oauth.simaster.ugm.ac.id/.well-known/openid-configuration (200) and\n  /.well-known/oauth-authorization-server (200), cross-checked against\n  https://oauth.simaster.ugm.ac.id/openapi.json. Not inferred — the institution declares these.\nx-operator: institution\napi: gadjah-mada-university:ugm-id\n\nsummary:\n  count: 5\n  model: OpenID Connect standard scopes plus two UGM-specific resource scopes.\n  granularity: coarse\n  note: >-\n    Five scopes for twenty operations. The three OIDC standard scopes govern identity claims; the\n    two UGM scopes (user.read, userDetail.read) split \"basic profile\" from \"full Simaster profile\".\n    There is no write scope anywhere in the server — every declared scope is read-only, and every\n    resource operation in the OpenAPI is a GET. No per-unit, per-faculty or per-system scoping\n \
  \   exists, so a client granted userDetail.read reads the full Simaster record for whatever\n    subject it is authorized for.\n\nscopes:\n- scope: openid\n  standard: OpenID Connect Core\n  description: Requests an id_token and enables the OIDC UserInfo endpoint.\n  grants_access_to:\n  - GET /userinfo\n- scope: profile\n  standard: OpenID Connect Core\n  description: >-\n    Basic profile claims - name, given_name, family_name, picture, preferred_username, plus UGM's\n    non-standard unit_id claim.\n  claims: [name, given_name, family_name, picture, preferred_username, unit_id]\n- scope: email\n  standard: OpenID Connect Core\n  description: Email claims.\n  claims: [email, email_verified]\n- scope: user.read\n  standard: UGM-specific\n  description: Read the authenticated subject's basic user profile.\n  grants_access_to:\n  - GET /api/me\n- scope: userDetail.read\n  standard: UGM-specific\n  description: >-\n    Read the full Simaster user record, and read another user's record by\
  \ username. The broadest\n    scope the server issues.\n  grants_access_to:\n  - GET /user/me\n  - GET /user/username/{username}\n\ngaps:\n- No write, update or delete scope exists on any UGM ID operation.\n- No scope documentation outside the discovery document — no prose page explains what each grants.\n- No consent-screen copy or scope description strings are published.\n- No incremental or step-up authorization is described.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gadjah-mada-university/refs/heads/main/scopes/gadjah-mada-university-scopes.yml
summary_line: 5 scopes
tags:
- University
- Higher Education
- Education
- Indonesia
- Research
- Identity Federation
- Authentication
- OpenID Connect
- OAuth
- Research Repository
- Scholarly Publishing
- OAI-PMH
- Library
token_urls: []
---
