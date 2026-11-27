---
api_specs:
- filename: google-shopping-accounts-api-openapi.yml
  format: yaml
  label: Google Content API for Shopping Accounts API
  slug: google-shopping-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-shopping/openapi/google-shopping-accounts-api-openapi.yml
authorization_urls:
- https://accounts.google.com/o/oauth2/auth
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Google Content API for Shopping Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Google Content API for Shopping publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Google Content API for Shopping API on a user''s behalf.


  Tokens are issued from https://oauth2.googleapis.com/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Google Content API for Shopping
provider_slug: google-shopping
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  source: openapi/google-shopping-accounts-api-openapi.yml
scope_count: 1
scope_names:
- https://www.googleapis.com/auth/content
scopes:
- description: Manage your product listings and accounts for Google Shopping
  flows:
  - authorizationCode
  scope: https://www.googleapis.com/auth/content
slug: google-shopping-scopes
source_filename: google-shopping-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/google-shopping-accounts-api-openapi.yml\nschemes:\n- name: oauth2\n  source: openapi/google-shopping-accounts-api-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\nscopes:\n- scope: https://www.googleapis.com/auth/content\n  description: Manage your product listings and accounts for Google Shopping\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/google-shopping-accounts-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/google-shopping/scopes/google-shopping-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- E-Commerce
- Google Shopping
- Merchant Center
- Product Listings
- Retail
- Shopping
token_bound: false
token_urls:
- https://oauth2.googleapis.com/token
---
