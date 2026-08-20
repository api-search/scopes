---
api_specs:
- filename: tu-delft-4tu-researchdata-openapi.yml
  format: yaml
  label: 4TU.ResearchData API
  slug: 4tu-researchdata
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tu-delft/refs/heads/main/openapi/tu-delft-4tu-researchdata-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Tu Delft Scopes
name_suffix: OAuth Scopes
note: TU Delft publishes no authorization scope vocabulary for any surface it operates. The only public institutional API, 4TU.ResearchData, authorizes with an opaque personal bearer token that carries no scope claims; there is no OAuth 2.0 authorization server, no OIDC discovery document, and no consent screen enumerating permissions. This file records the absence deliberately rather than leaving the slot empty — an empty scopes/ directory reads as "not checked", and this was checked.
overview: 'Delft University of Technology uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Delft University of Technology
provider_slug: tu-delft
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: tu-delft-scopes
source_filename: tu-delft-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: >-\n  https://data.4tu.nl/v2/account/articles (HTTP 403), djehuty docs/api.md, and a check for\n  https://data.4tu.nl/.well-known/openid-configuration and /.well-known/oauth-authorization-server\n  (both HTTP 404, \"This resource does not exist.\").\nx-operator: institution\nscopes_published: false\nnote: >-\n  TU Delft publishes no authorization scope vocabulary for any surface it operates. The only\n  public institutional API, 4TU.ResearchData, authorizes with an opaque personal bearer token\n  that carries no scope claims; there is no OAuth 2.0 authorization server, no OIDC discovery\n  document, and no consent screen enumerating permissions. This file records the absence\n  deliberately rather than leaving the slot empty — an empty scopes/ directory reads as\n  \"not checked\", and this was checked.\nscopes: []\nauthorization_model:\n  type: all-or-nothing-token\n  granularity: account\n  delegation: none\n  consent_surface:\
  \ none\n  revocation: Token can be revoked from the depositor dashboard; no programmatic revocation endpoint found.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-delft/refs/heads/main/scopes/tu-delft-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Technical University
- Research Data
- Open Access
- Identity Federation
- Research Repository
- Research Computing
- 4TU.Federation
- Netherlands
- Europe
token_urls: []
---
