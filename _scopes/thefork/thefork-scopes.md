---
api_specs:
- filename: thefork-b2b-openapi.yml
  format: yaml
  label: TheFork B2B API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-b2b-openapi.yml
- filename: thefork-pos-openapi.yml
  format: yaml
  label: TheFork POS API
  slug: pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/openapi/thefork-pos-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.thefork.io/B2B-API/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Thefork Scopes
name_suffix: OAuth Scopes
note: TheFork does not use or document OAuth scopes; access is granted via an Auth0 client credentials flow (client_id/client_secret exchanged for a bearer token), with POS/Partners access controlled by API keys rather than scopes (https://docs.thefork.io/B2B-API/authentication).
overview: 'TheFork uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.thefork.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: TheFork
provider_slug: thefork
schemes:
- description: Auth0 OAuth 2.0 client credentials flow. Exchange client_id and client_secret for a bearer token at https://auth.thefork.io/oauth/token with audience https://api.thefork.io. Tokens expire after 8600 seconds.
  flows:
  - flow: clientCredentials
    tokenUrl: https://auth.thefork.io/oauth/token
  name: OAuth2ClientCredentials
  source: openapi/thefork-b2b-openapi.yml
scope_count: 0
scope_names: []
scopes: []
slug: thefork-scopes
source_filename: thefork-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/thefork-b2b-openapi.yml\ndocs: https://docs.thefork.io/B2B-API/authentication\nnote: TheFork does not use or document OAuth scopes; access is granted via an Auth0\n  client credentials flow (client_id/client_secret exchanged for a bearer token),\n  with POS/Partners access controlled by API keys rather than scopes\n  (https://docs.thefork.io/B2B-API/authentication).\nschemes:\n- name: OAuth2ClientCredentials\n  source: openapi/thefork-b2b-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.thefork.io/oauth/token\n  description: Auth0 OAuth 2.0 client credentials flow. Exchange client_id and client_secret\n    for a bearer token at https://auth.thefork.io/oauth/token with audience https://api.thefork.io.\n    Tokens expire after 8600 seconds.\nscopes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thefork/refs/heads/main/scopes/thefork-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Restaurant
- Reservations
- Booking
- Dining
- Point Of Sale
- Marketplace
token_urls:
- https://auth.thefork.io/oauth/token
---
