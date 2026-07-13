---
api_specs:
- filename: leafly-menu-integration-openapi.yml
  format: yaml
  label: Leafly Menu Integration API
  slug: leafly-menu-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leafly/refs/heads/main/openapi/leafly-menu-integration-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.leafly.io/menu-integration-docs/v2.html
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Leafly Scopes
name_suffix: OAuth Scopes
note: Leafly's Menu Integration API V2 uses the OAuth2 client credentials grant with no published scopes - the upstream OpenAPI (https://docs.leafly.io/menu-integration-docs/v2.json) declares an empty scopes map and access is instead tied to a Leafly-issued menu_integration_key identifying the retailer.
overview: 'Leafly uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://api.leafly.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Leafly
provider_slug: leafly
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.leafly.com/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/leafly-menu-integration-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: leafly-scopes
source_filename: leafly-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/leafly-menu-integration-openapi.yml\ndocs: https://docs.leafly.io/menu-integration-docs/v2.html\nnote: Leafly's Menu Integration API V2 uses the OAuth2 client credentials grant\n  with no published scopes - the upstream OpenAPI (https://docs.leafly.io/menu-integration-docs/v2.json)\n  declares an empty scopes map and access is instead tied to a Leafly-issued\n  menu_integration_key identifying the retailer.\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/leafly-menu-integration-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.leafly.com/oauth/token\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leafly/refs/heads/main/scopes/leafly-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Cannabis
- Dispensary
- Menu Sync
- POS Integration
- Retail
- Marketplace
- Strains
- Ecommerce
token_urls:
- https://api.leafly.com/oauth/token
---
