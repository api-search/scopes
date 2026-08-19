---
api_specs:
- filename: lafourchette-b2b-api-openapi.yml
  format: yaml
  label: TheFork B2B API
  slug: thefork-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-b2b-api-openapi.yml
- filename: lafourchette-pos-api-openapi.yml
  format: yaml
  label: TheFork POS API v1
  slug: thefork-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/openapi/lafourchette-pos-api-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.thefork.io/B2B-API/authentication
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: probed
name: Lafourchette Scopes
name_suffix: OAuth Scopes
note: 'TheFork''s B2B API authenticates with an Auth0 client-credentials grant against audience https://api.thefork.io. TheFork documents NO API-specific scopes and its published operation objects carry no oauth2 securityScheme, so there is no scope reference page to harvest — entitlements are set per partner contract when the integrations team issues the client_id/client_secret. The scopes listed below are the standard OIDC identity scopes advertised by the Auth0 tenant''s own discovery document; they are recorded because they were probed, not because they gate the B2B API. Treat scope granularity for this API as: none published.'
overview: 'LaFourchette uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from https://auth.thefork.io/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: LaFourchette
provider_slug: lafourchette
schemes:
- flows:
  - audience: https://api.thefork.io
    flow: clientCredentials
    scopes: {}
    tokenUrl: https://auth.thefork.io/oauth/token
  name: Auth0ClientCredentials
  source: https://docs.thefork.io/B2B-API/authentication
scope_count: 0
scope_names: []
scopes: []
slug: lafourchette-scopes
source_filename: lafourchette-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://auth.thefork.io/.well-known/openid-configuration\ndocs: https://docs.thefork.io/B2B-API/authentication\nnote: >-\n  TheFork's B2B API authenticates with an Auth0 client-credentials grant against audience\n  https://api.thefork.io. TheFork documents NO API-specific scopes and its published operation\n  objects carry no oauth2 securityScheme, so there is no scope reference page to harvest — entitlements\n  are set per partner contract when the integrations team issues the client_id/client_secret. The\n  scopes listed below are the standard OIDC identity scopes advertised by the Auth0 tenant's own\n  discovery document; they are recorded because they were probed, not because they gate the B2B API.\n  Treat scope granularity for this API as: none published.\nschemes:\n- name: Auth0ClientCredentials\n  source: https://docs.thefork.io/B2B-API/authentication\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.thefork.io/oauth/token\n\
  \    audience: https://api.thefork.io\n    scopes: {}\napi_scopes_published: false\napi_scope_count: 0\ntenant_scopes_supported:\n- scope: openid\n  kind: oidc-identity\n- scope: profile\n  kind: oidc-identity\n- scope: offline_access\n  kind: oidc-identity\n- scope: name\n  kind: oidc-identity\n- scope: given_name\n  kind: oidc-identity\n- scope: family_name\n  kind: oidc-identity\n- scope: nickname\n  kind: oidc-identity\n- scope: email\n  kind: oidc-identity\n- scope: email_verified\n  kind: oidc-identity\n- scope: picture\n  kind: oidc-identity\n- scope: created_at\n  kind: oidc-identity\n- scope: identities\n  kind: oidc-identity\n- scope: phone\n  kind: oidc-identity\n- scope: address\n  kind: oidc-identity\nx-evidence:\n- url: https://auth.thefork.io/.well-known/openid-configuration\n  status: 200\n- url: https://docs.thefork.io/B2B-API/authentication\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lafourchette/refs/heads/main/scopes/lafourchette-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Company
- Consumer
- Restaurants
- Reservations
- Booking
- Hospitality
- Point of Sale
- Reviews
- Marketplace
- Travel and Dining
- Webhooks
- France
token_urls:
- https://auth.thefork.io/oauth/token
---
