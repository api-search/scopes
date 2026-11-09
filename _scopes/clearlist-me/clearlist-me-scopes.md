---
api_specs:
- filename: clearlist-me-account-api-openapi.yml
  format: yaml
  label: ClearList Account API
  slug: clearlist-me-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-account-api-openapi.yml
- filename: clearlist-me-jobs-api-openapi.yml
  format: yaml
  label: ClearList Jobs API
  slug: clearlist-me-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-jobs-api-openapi.yml
- filename: clearlist-me-listings-api-openapi.yml
  format: yaml
  label: ClearList Listings API
  slug: clearlist-me-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-listings-api-openapi.yml
- filename: clearlist-me-onboarding-api-openapi.yml
  format: yaml
  label: ClearList Onboarding API
  slug: clearlist-me-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-onboarding-api-openapi.yml
- filename: clearlist-me-orders-api-openapi.yml
  format: yaml
  label: ClearList Orders API
  slug: clearlist-me-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-orders-api-openapi.yml
- filename: clearlist-me-publishing-api-openapi.yml
  format: yaml
  label: ClearList Publishing API
  slug: clearlist-me-publishing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-publishing-api-openapi.yml
- filename: clearlist-me-scheduling-api-openapi.yml
  format: yaml
  label: ClearList Scheduling API
  slug: clearlist-me-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-scheduling-api-openapi.yml
- filename: clearlist-me-system-api-openapi.yml
  format: yaml
  label: ClearList System API
  slug: clearlist-me-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clearlist-me/openapi/clearlist-me-system-api-openapi.yml
authorization_urls:
- https://clearlist.me/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Clearlist Me Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'ClearList publishes 2 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the ClearList API on a user''s behalf.


  Tokens are issued from https://clearlist.me/api/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: ClearList
provider_slug: clearlist-me
schemes:
- description: 'OAuth 2.1 authorization code flow. PKCE with code_challenge_method=S256 is required; public clients only (token_endpoint_auth_method none). Access tokens are `cl_<64-hex>` and are sent as `Authorization: Bearer <token>` (X-ClearList-API-Key also works). Operations that change state require the `write` scope; a grant without it gets 403. Reading needs no specific scope, so a `write`-only grant can also read.'
  flows:
  - authorizationUrl: https://clearlist.me/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://clearlist.me/api/oauth/token
  name: oauth2
  source: openapi/clearlist-me-openapi.json
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read listings, reservations, conversations, page stats and plan status.
  flows:
  - authorizationCode
  scope: read
- description: Create, edit, delete and publish listings; reply to buyers; share an address through the confirmed flow; set availability; create payment links.
  flows:
  - authorizationCode
  scope: write
slug: clearlist-me-scopes
source_filename: clearlist-me-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/clearlist-me-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/clearlist-me-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://clearlist.me/oauth/authorize\n    tokenUrl: https://clearlist.me/api/oauth/token\n  description: 'OAuth 2.1 authorization code flow. PKCE with code_challenge_method=S256 is required;\n    public clients only (token_endpoint_auth_method none). Access tokens are `cl_<64-hex>` and\n    are sent as `Authorization: Bearer <token>` (X-ClearList-API-Key also works). Operations\n    that change state require the `write` scope; a grant without it gets 403. Reading needs\n    no specific scope, so a `write`-only grant can also read.'\nscopes:\n- scope: read\n  description: Read listings, reservations, conversations, page stats and plan status.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/clearlist-me-openapi.json\n- scope: write\n  description: Create,\
  \ edit, delete and publish listings; reply to buyers; share an address\n    through the confirmed flow; set availability; create payment links.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/clearlist-me-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/clearlist-me/scopes/clearlist-me-scopes.yml
summary_line: 2 scopes · authorizationCode
tags:
- Artificial Intelligence
- Resale
- Marketplace
- Automation
- E-Commerce
- Company
token_bound: false
token_urls:
- https://clearlist.me/api/oauth/token
---
