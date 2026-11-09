---
api_specs:
- filename: cartviral-com-account-api-openapi.yml
  format: yaml
  label: CartViral Account API
  slug: cartviral-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-account-api-openapi.yml
- filename: cartviral-com-carousels-api-openapi.yml
  format: yaml
  label: CartViral Carousels API
  slug: cartviral-com-carousels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-carousels-api-openapi.yml
- filename: cartviral-com-characters-api-openapi.yml
  format: yaml
  label: CartViral Characters API
  slug: cartviral-com-characters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-characters-api-openapi.yml
- filename: cartviral-com-clips-api-openapi.yml
  format: yaml
  label: CartViral Clips API
  slug: cartviral-com-clips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-clips-api-openapi.yml
- filename: cartviral-com-create-api-openapi.yml
  format: yaml
  label: CartViral Create API
  slug: cartviral-com-create-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-create-api-openapi.yml
- filename: cartviral-com-creations-api-openapi.yml
  format: yaml
  label: CartViral Creations API
  slug: cartviral-com-creations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-creations-api-openapi.yml
- filename: cartviral-com-media-api-openapi.yml
  format: yaml
  label: CartViral Media API
  slug: cartviral-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-media-api-openapi.yml
- filename: cartviral-com-offers-api-openapi.yml
  format: yaml
  label: CartViral Offers API
  slug: cartviral-com-offers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-offers-api-openapi.yml
- filename: cartviral-com-photos-api-openapi.yml
  format: yaml
  label: CartViral Photos API
  slug: cartviral-com-photos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-photos-api-openapi.yml
- filename: cartviral-com-pitches-api-openapi.yml
  format: yaml
  label: CartViral Pitches API
  slug: cartviral-com-pitches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-pitches-api-openapi.yml
- filename: cartviral-com-products-api-openapi.yml
  format: yaml
  label: CartViral Products API
  slug: cartviral-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-products-api-openapi.yml
- filename: cartviral-com-static-ads-api-openapi.yml
  format: yaml
  label: CartViral Static Ads API
  slug: cartviral-com-static-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cartviral-com/openapi/cartviral-com-static-ads-api-openapi.yml
authorization_urls:
- https://app.cartviral.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Cartviral Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'CartViral publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the CartViral API on a user''s behalf.


  Tokens are issued from https://app.cartviral.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: CartViral
provider_slug: cartviral-com
schemes:
- flows:
  - authorizationUrl: https://app.cartviral.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.cartviral.com/oauth/token
  name: oauth
  source: openapi/cartviral-com-openapi.json
scope_count: 1
scope_names:
- mcp
scopes:
- description: Use your CartViral account
  flows:
  - authorizationCode
  scope: mcp
slug: cartviral-com-scopes
source_filename: cartviral-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/cartviral-com-openapi.json\nschemes:\n- name: oauth\n  source: openapi/cartviral-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.cartviral.com/oauth/authorize\n    tokenUrl: https://app.cartviral.com/oauth/token\nscopes:\n- scope: mcp\n  description: Use your CartViral account\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/cartviral-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cartviral-com/scopes/cartviral-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
- Artificial Intelligence
- E-Commerce
- Video Generation
- Marketing
token_bound: false
token_urls:
- https://app.cartviral.com/oauth/token
---
