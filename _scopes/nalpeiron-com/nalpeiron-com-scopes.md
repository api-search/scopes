---
api_specs:
- filename: nalpeiron-com-openapi-generated.yml
  format: yaml
  label: Nalpeiron API
  slug: nalpeiron-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nalpeiron-com/openapi/_ae-authored/nalpeiron-com-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Nalpeiron Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'Nalpeiron uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from $NALPEIRON_TOKEN_URL.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Nalpeiron
provider_slug: nalpeiron-com
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: $NALPEIRON_TOKEN_URL
  name: client_credentials
  source: openapi/nalpeiron-com-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: nalpeiron-com-scopes
source_filename: nalpeiron-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: none\nsource: openapi/nalpeiron-com-openapi-generated.yml\nschemes:\n- name: client_credentials\n  source: openapi/nalpeiron-com-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: $NALPEIRON_TOKEN_URL\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/nalpeiron-com/scopes/nalpeiron-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Software Licensing
- Monetization
- Software-as-a-Service
- IoT
- Entitlement Management
token_bound: false
token_urls:
- $NALPEIRON_TOKEN_URL
---
