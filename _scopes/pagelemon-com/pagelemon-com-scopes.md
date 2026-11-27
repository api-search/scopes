---
api_specs:
- filename: pagelemon-com-account-api-openapi.yml
  format: yaml
  label: Page Lemon Account API
  slug: pagelemon-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-account-api-openapi.yml
- filename: pagelemon-com-automations-api-openapi.yml
  format: yaml
  label: Page Lemon Automations API
  slug: pagelemon-com-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-automations-api-openapi.yml
- filename: pagelemon-com-bookings-api-openapi.yml
  format: yaml
  label: Page Lemon Bookings API
  slug: pagelemon-com-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-bookings-api-openapi.yml
- filename: pagelemon-com-lists-api-openapi.yml
  format: yaml
  label: Page Lemon Lists API
  slug: pagelemon-com-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-lists-api-openapi.yml
- filename: pagelemon-com-pages-api-openapi.yml
  format: yaml
  label: Page Lemon Pages API
  slug: pagelemon-com-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-pages-api-openapi.yml
- filename: pagelemon-com-payments-api-openapi.yml
  format: yaml
  label: Page Lemon Payments API
  slug: pagelemon-com-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-payments-api-openapi.yml
- filename: pagelemon-com-platform-api-openapi.yml
  format: yaml
  label: Page Lemon Platform API
  slug: pagelemon-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-platform-api-openapi.yml
- filename: pagelemon-com-rules-api-openapi.yml
  format: yaml
  label: Page Lemon Rules API
  slug: pagelemon-com-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-rules-api-openapi.yml
- filename: pagelemon-com-sign-in-api-openapi.yml
  format: yaml
  label: Page Lemon Sign In API
  slug: pagelemon-com-sign-in-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-sign-in-api-openapi.yml
- filename: pagelemon-com-views-api-openapi.yml
  format: yaml
  label: Page Lemon Views API
  slug: pagelemon-com-views-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagelemon-com/openapi/pagelemon-com-views-api-openapi.yml
authorization_urls:
- https://dash.pagelemon.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Page Lemon Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Page Lemon publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Page Lemon API on a user''s behalf.


  Tokens are issued from https://dash.pagelemon.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Page Lemon
provider_slug: pagelemon-com
schemes:
- description: 'OAuth 2.0 authorization code with PKCE (S256), as AI connectors sign in (docs/contract/mcp-oauth.md); metadata at https://dash.pagelemon.com/.well-known/oauth-authorization-server. For the MCP server only: a connector token is refused straight on REST, so no operation here lists it.'
  flows:
  - authorizationUrl: https://dash.pagelemon.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://dash.pagelemon.com/oauth/token
  name: oauth2
  source: openapi/pagelemon-com-openapi.json
scope_count: 4
scope_names:
- data
- deploy
- manage
- read
scopes:
- description: Read customer data (form replies, users, orders)
  flows:
  - authorizationCode
  scope: data
- description: Publish versions and upload files
  flows:
  - authorizationCode
  scope: deploy
- description: Change settings, people and integrations
  flows:
  - authorizationCode
  scope: manage
- description: Read sites, lists and settings
  flows:
  - authorizationCode
  scope: read
slug: pagelemon-com-scopes
source_filename: pagelemon-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/pagelemon-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/pagelemon-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://dash.pagelemon.com/oauth/authorize\n    tokenUrl: https://dash.pagelemon.com/oauth/token\n  description: 'OAuth 2.0 authorization code with PKCE (S256), as AI connectors sign in (docs/contract/mcp-oauth.md);\n    metadata at https://dash.pagelemon.com/.well-known/oauth-authorization-server. For the MCP\n    server only: a connector token is refused straight on REST, so no operation here lists it.'\nscopes:\n- scope: data\n  description: Read customer data (form replies, users, orders)\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pagelemon-com-openapi.json\n- scope: deploy\n  description: Publish versions and upload files\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pagelemon-com-openapi.json\n- scope: manage\n  description: Change\
  \ settings, people and integrations\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pagelemon-com-openapi.json\n- scope: read\n  description: Read sites, lists and settings\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/pagelemon-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/pagelemon-com/scopes/pagelemon-com-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Website Builder
- Booking
- Payments
- Integration
- Developers
token_bound: false
token_urls:
- https://dash.pagelemon.com/oauth/token
---
