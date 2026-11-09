---
api_specs:
- filename: firetail-openapi-generated.yml
  format: yaml
  label: FireTail API
  slug: firetail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firetail/openapi/_ae-authored/firetail-openapi-generated.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: none
name: Firetail Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'FireTail uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.saas.eu-west-1.prod.firetail.app/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FireTail
provider_slug: firetail
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.saas.eu-west-1.prod.firetail.app/oauth/token
  name: OAuth_2.0_client_credentials
  source: openapi/firetail-openapi-generated.yml
scope_count: 0
scope_names: []
scopes: []
slug: firetail-scopes
source_filename: firetail-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: none\nsource: openapi/firetail-openapi-generated.yml\nschemes:\n- name: OAuth_2.0_client_credentials\n  source: openapi/firetail-openapi-generated.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.saas.eu-west-1.prod.firetail.app/oauth/token\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/firetail/scopes/firetail-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Security
- Governance
- Platform
- Cloud
token_bound: false
token_urls:
- https://api.saas.eu-west-1.prod.firetail.app/oauth/token
---
