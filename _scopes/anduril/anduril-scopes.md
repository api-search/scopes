---
api_specs:
- filename: anduril-openapi.yml
  format: yaml
  label: Anduril Lattice SDK
  slug: lattice-sdk
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/openapi/anduril-openapi.yml
authorization_urls: []
description: ''
docs: https://developer.anduril.com/reference/rest/oauth/get-token
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Anduril Scopes
name_suffix: OAuth Scopes
note: Anduril Lattice uses the OAuth 2.0 client credentials flow with no published scope catalog; the token endpoint accepts no scope parameter and access is governed by partner-gated client credentials (https://developer.anduril.com/reference/rest/oauth/get-token).
overview: 'Anduril Industries uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.developer.anduril.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Anduril Industries
provider_slug: anduril
schemes:
- description: OAuth 2.0 client credentials flow for service-to-service access.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.developer.anduril.com/oauth/token
  name: oauth2ClientCredentials
  source: openapi/anduril-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: anduril-scopes
source_filename: anduril-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anduril-openapi.yml\ndocs: https://developer.anduril.com/reference/rest/oauth/get-token\nnote: Anduril Lattice uses the OAuth 2.0 client credentials flow with no published\n  scope catalog; the token endpoint accepts no scope parameter and access is governed\n  by partner-gated client credentials (https://developer.anduril.com/reference/rest/oauth/get-token).\nschemes:\n- name: oauth2ClientCredentials\n  source: openapi/anduril-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.developer.anduril.com/oauth/token\n  description: OAuth 2.0 client credentials flow for service-to-service access.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anduril/refs/heads/main/scopes/anduril-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Defense
- Autonomy
- Lattice
- Command and Control
- C2
- Sensors
- Effectors
- Counter-UAS
- Unmanned Systems
- Mission Software
- Edge AI
- ITAR
token_urls:
- https://api.developer.anduril.com/oauth/token
---
