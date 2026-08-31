---
api_specs:
- filename: university-of-sheffield-sheffield-solar-api-openapi.yml
  format: yaml
  label: Sheffield Solar API
  slug: sheffield-solar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/openapi/university-of-sheffield-sheffield-solar-api-openapi.yml
authorization_urls: []
description: 'The University of Sheffield''s own Sheffield Solar API declares an OAuth2 password flow but publishes an EMPTY scopes object — there is no scope vocabulary to record. Authorization is coarse: an operation is either open, or it requires an authenticated user, or it requires an administrator. This file records that absence rather than inventing scopes to fill it.'
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: derived
name: University Of Sheffield Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'University of Sheffield uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.solar.sheffield.ac.uk/auth/jwt/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: University of Sheffield
provider_slug: university-of-sheffield
schemes:
- flows:
  - flow: password
    scopes_declared: 0
    tokenUrl: https://api.solar.sheffield.ac.uk/auth/jwt/login
  name: OAuth2PasswordBearer
scope_count: 0
scope_names: []
scopes: []
slug: university-of-sheffield-scopes
source_filename: university-of-sheffield-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\ngenerated: '2026-08-30'\nmethod: derived\nsource: openapi/university-of-sheffield-sheffield-solar-api-openapi.yml\nprovider: University of Sheffield\nx-operator: institution\ndescription: >-\n  The University of Sheffield's own Sheffield Solar API declares an OAuth2 password\n  flow but publishes an EMPTY scopes object — there is no scope vocabulary to record.\n  Authorization is coarse: an operation is either open, or it requires an\n  authenticated user, or it requires an administrator. This file records that\n  absence rather than inventing scopes to fill it.\nschemes:\n  - name: OAuth2PasswordBearer\n    flows:\n      - flow: password\n        tokenUrl: https://api.solar.sheffield.ac.uk/auth/jwt/login\n        scopes_declared: 0\nscopes: []\ncoarse_authorization_tiers:\n  - tier: open\n    description: No credential. PV_Live and PV_Live_EU read endpoints, and the gsp/pes/nuts lists.\n    evidence:\n      url: https://api.solar.sheffield.ac.uk/pvlive/api/v4/gsp/0\n\
  \      status: 200\n  - tier: registered-user\n    description: Requires a registered identifier (X-User-Id header) or a JWT. PV_Forecast endpoints, /users/me.\n    evidence:\n      url: https://api.solar.sheffield.ac.uk/pvforecast/api/v4/gsp/0\n      status: 401\n  - tier: administrator\n    description: The /admin operations, which issue and revoke user tokens.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-sheffield/refs/heads/main/scopes/university-of-sheffield-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Open Access
- OAI-PMH
- Identity Federation
- Solar Energy
- Energy Data
- Research Computing
token_urls:
- https://api.solar.sheffield.ac.uk/auth/jwt/login
---
