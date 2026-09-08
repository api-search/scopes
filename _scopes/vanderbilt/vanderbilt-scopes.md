---
api_specs:
- filename: vanderbilt-television-news-archive-openapi.yml
  format: yaml
  label: Vanderbilt Television News Archive API
  slug: television-news-archive
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanderbilt/refs/heads/main/openapi/vanderbilt-television-news-archive-openapi.yml
- filename: vanderbilt-sparql-openapi.yml
  format: yaml
  label: Vanderbilt Libraries SPARQL Endpoint
  slug: sparql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanderbilt/refs/heads/main/openapi/vanderbilt-sparql-openapi.yml
authorization_urls: []
description: OAuth 2.0 / OpenID Connect scopes advertised by Vanderbilt's federated identity providers. Read directly from each provider's live OpenID Connect Discovery document; nothing here is inferred. Vanderbilt's three public read APIs are unauthenticated and define no scopes of their own.
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: probed
name: Vanderbilt Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Vanderbilt University uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Vanderbilt University
provider_slug: vanderbilt
schemes: []
scope_count: 0
scope_names: []
scopes: []
slug: vanderbilt-scopes
source_filename: vanderbilt-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "---\nname: Vanderbilt University — OAuth Scopes\ndescription: >-\n  OAuth 2.0 / OpenID Connect scopes advertised by Vanderbilt's federated identity providers.\n  Read directly from each provider's live OpenID Connect Discovery document; nothing here is\n  inferred. Vanderbilt's three public read APIs are unauthenticated and define no scopes of\n  their own.\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  https://onevu.vanderbilt.edu/.well-known/openid-configuration and\n  https://login.microsoftonline.com/vanderbilt.edu/v2.0/.well-known/openid-configuration,\n  both fetched 2026-09-01, HTTP 200.\nproviders:\n  - provider: Vanderbilt Okta (OneVU)\n    operator: federation\n    issuer: https://onevu.vanderbilt.edu\n    scopes:\n      - { scope: openid, description: OpenID Connect authentication request. }\n      - { scope: profile, description: Basic profile claims. }\n      - { scope: email, description: Email address and verification status. }\n      - { scope: address,\
  \ description: Postal address claim. }\n      - { scope: phone, description: Phone number claim. }\n      - { scope: offline_access, description: Refresh token issuance. }\n      - { scope: groups, description: Okta group membership claim. }\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - 'urn:ietf:params:oauth:grant-type:device_code'\n      - 'urn:openid:params:grant-type:ciba'\n  - provider: Vanderbilt Microsoft Entra ID\n    operator: federation\n    issuer: https://login.microsoftonline.com/ba5a7f39-e3be-4ab3-b450-67fa80faecad/v2.0\n    scopes:\n      - { scope: openid, description: OpenID Connect authentication request. }\n      - { scope: profile, description: Basic profile claims. }\n      - { scope: email, description: Email address claim. }\n      - { scope: offline_access, description: Refresh token issuance. }\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanderbilt/refs/heads/main/scopes/vanderbilt-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- University
- Higher Education
- Education
- Private Research University
- Research Data
- Institutional Repository
- Linked Data
- SPARQL
- Digital Collections
- Television News Archive
- Identity Federation
- Library
- Nashville
- Tennessee
- United States
token_urls: []
---
