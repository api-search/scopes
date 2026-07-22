---
api_specs:
- filename: socialbakers-emplifi-public-api-openapi.yml
  format: yaml
  label: Emplifi (Socialbakers) Public API
  slug: emplifi-socialbakers-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/openapi/socialbakers-emplifi-public-api-openapi.yml
authorization_urls:
- https://api.emplifi.io/oauth2/0/auth
description: ''
docs: https://api.emplifi.io/
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: searched
name: Socialbakers Scopes
name_suffix: OAuth Scopes
note: The Emplifi (Socialbakers) Public API v3 supports OAuth 2.0 authorization code flow (Custom integration in Emplifi Settings). The published documentation does not enumerate a named OAuth scope catalog — access is governed by the integration's granted product permissions rather than request-time scopes. Recorded here so the OAuth surface is discoverable; no fabricated scope strings are included.
overview: 'Socialbakers uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.emplifi.io/oauth2/0/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Socialbakers
provider_slug: socialbakers
schemes:
- flows:
  - authorizationUrl: https://api.emplifi.io/oauth2/0/auth
    flow: authorizationCode
    revocationUrl: https://api.emplifi.io/oauth2/0/token/revocation
    tokenUrl: https://api.emplifi.io/oauth2/0/token
  name: oauth2
  source: https://api.emplifi.io/
scope_count: 0
scope_names: []
scopes: []
slug: socialbakers-scopes
source_filename: socialbakers-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.emplifi.io/\ndocs: https://api.emplifi.io/\nnote: >-\n  The Emplifi (Socialbakers) Public API v3 supports OAuth 2.0 authorization\n  code flow (Custom integration in Emplifi Settings). The published\n  documentation does not enumerate a named OAuth scope catalog — access is\n  governed by the integration's granted product permissions rather than\n  request-time scopes. Recorded here so the OAuth surface is discoverable;\n  no fabricated scope strings are included.\nschemes:\n  - name: oauth2\n    source: https://api.emplifi.io/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.emplifi.io/oauth2/0/auth\n        tokenUrl: https://api.emplifi.io/oauth2/0/token\n        revocationUrl: https://api.emplifi.io/oauth2/0/token/revocation\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socialbakers/refs/heads/main/scopes/socialbakers-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Marketing
- Social Media
- Analytics
- Social Media Analytics
- Social Listening
- Marketing Analytics
- Digital Asset Management
- Customer Care
- Emplifi
token_urls:
- https://api.emplifi.io/oauth2/0/token
---
