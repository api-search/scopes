---
api_specs:
- filename: dystro-dev-accounts-api-openapi.yml
  format: yaml
  label: dystro-dev Accounts API
  slug: dystro-dev-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-accounts-api-openapi.yml
- filename: dystro-dev-analytics-api-openapi.yml
  format: yaml
  label: dystro-dev Analytics API
  slug: dystro-dev-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-analytics-api-openapi.yml
- filename: dystro-dev-api-keys-api-openapi.yml
  format: yaml
  label: dystro-dev API Keys API
  slug: dystro-dev-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-api-keys-api-openapi.yml
- filename: dystro-dev-campaigns-api-openapi.yml
  format: yaml
  label: dystro-dev Campaigns API
  slug: dystro-dev-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-campaigns-api-openapi.yml
- filename: dystro-dev-connect-api-openapi.yml
  format: yaml
  label: dystro-dev Connect API
  slug: dystro-dev-connect-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-connect-api-openapi.yml
- filename: dystro-dev-inbox-api-openapi.yml
  format: yaml
  label: dystro-dev Inbox API
  slug: dystro-dev-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-inbox-api-openapi.yml
- filename: dystro-dev-media-api-openapi.yml
  format: yaml
  label: dystro-dev Media API
  slug: dystro-dev-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-media-api-openapi.yml
- filename: dystro-dev-meta-api-openapi.yml
  format: yaml
  label: dystro-dev Meta API
  slug: dystro-dev-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-meta-api-openapi.yml
- filename: dystro-dev-posts-api-openapi.yml
  format: yaml
  label: dystro-dev Posts API
  slug: dystro-dev-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-posts-api-openapi.yml
- filename: dystro-dev-queue-api-openapi.yml
  format: yaml
  label: dystro-dev Queue API
  slug: dystro-dev-queue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-queue-api-openapi.yml
- filename: dystro-dev-webhooks-api-openapi.yml
  format: yaml
  label: dystro-dev Webhooks API
  slug: dystro-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dystro-dev/openapi/dystro-dev-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: derived
name: Dystro Dev Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'dystro-dev publishes 6 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the dystro-dev API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: dystro-dev
provider_slug: dystro-dev
schemes: []
scope_count: 6
scope_names:
- accounts:write
- analytics:read
- media:write
- posts:write
- posts:read
- accounts:read
scopes:
- description: Write access to account resources.
  flows: []
  scope: accounts:write
- description: Read access to analytics data.
  flows: []
  scope: analytics:read
- description: Write access to media items.
  flows: []
  scope: media:write
- description: Write access to posts.
  flows: []
  scope: posts:write
- description: Read access to posts.
  flows: []
  scope: posts:read
- description: Read access to account information.
  flows: []
  scope: accounts:read
slug: dystro-dev-scopes
source_filename: dystro-dev-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/dystro-dev-openapi.json\nscopes:\n  - name: accounts:write\n    description: Write access to account resources.\n  - name: analytics:read\n    description: Read access to analytics data.\n  - name: media:write\n    description: Write access to media items.\n  - name: posts:write\n    description: Write access to posts.\n  - name: posts:read\n    description: Read access to posts.\n  - name: accounts:read\n    description: Read access to account information.\n"
source_yaml_url: https://artifacts.apis.io/dystro-dev/scopes/dystro-dev-scopes.yml
summary_line: 6 scopes
tags:
- Company
- API
- Developer
- Technology
- Integration
token_bound: false
token_urls: []
---
