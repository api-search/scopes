---
api_specs:
- filename: tessio-eu-age-verification-api-openapi.yml
  format: yaml
  label: tessio-eu Age Verification API
  slug: tessio-eu-age-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessio-eu/openapi/tessio-eu-age-verification-api-openapi.yml
- filename: tessio-eu-stats-api-openapi.yml
  format: yaml
  label: tessio-eu Stats API
  slug: tessio-eu-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessio-eu/openapi/tessio-eu-stats-api-openapi.yml
- filename: tessio-eu-webhooks-api-openapi.yml
  format: yaml
  label: tessio-eu Webhooks API
  slug: tessio-eu-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tessio-eu/openapi/tessio-eu-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Tessio Eu Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'tessio-eu publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the tessio-eu API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: tessio-eu
provider_slug: tessio-eu
schemes: []
scope_count: 2
scope_names:
- full
- stats:read
scopes:
- description: Full access to all /v1 routes for the project
  flows: []
  scope: full
- description: Read-only access to /v1/stats/* endpoints
  flows: []
  scope: stats:read
slug: tessio-eu-scopes
source_filename: tessio-eu-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://tessio.eu/docs/api/\nscopes:\n  - name: full\n    description: \"Full access to all /v1 routes for the project\"\n  - name: stats:read\n    description: \"Read-only access to /v1/stats/* endpoints\"\n"
source_yaml_url: https://artifacts.apis.io/tessio-eu/scopes/tessio-eu-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Age Verification
- EU
- Identity
token_bound: false
token_urls: []
---
