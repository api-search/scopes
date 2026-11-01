---
api_specs:
- filename: yappy-biz-batch-api-openapi.yml
  format: yaml
  label: yappy-biz Batch API
  slug: yappy-biz-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-batch-api-openapi.yml
- filename: yappy-biz-commerce-api-openapi.yml
  format: yaml
  label: yappy-biz Commerce API
  slug: yappy-biz-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-commerce-api-openapi.yml
- filename: yappy-biz-discovery-api-openapi.yml
  format: yaml
  label: yappy-biz Discovery API
  slug: yappy-biz-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-discovery-api-openapi.yml
- filename: yappy-biz-documentation-api-openapi.yml
  format: yaml
  label: yappy-biz Documentation API
  slug: yappy-biz-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-documentation-api-openapi.yml
- filename: yappy-biz-exports-api-openapi.yml
  format: yaml
  label: yappy-biz Exports API
  slug: yappy-biz-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-exports-api-openapi.yml
- filename: yappy-biz-product-api-openapi.yml
  format: yaml
  label: yappy-biz Product API
  slug: yappy-biz-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-product-api-openapi.yml
- filename: yappy-biz-releases-api-openapi.yml
  format: yaml
  label: yappy-biz Releases API
  slug: yappy-biz-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/yappy-biz/openapi/yappy-biz-releases-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Yappy Biz Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'yappy-biz publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the yappy-biz API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: yappy-biz
provider_slug: yappy-biz
schemes: []
scope_count: 5
scope_names:
- read:releases
- read:docs
- read:pricing
- read:faq
- export:docs
scopes:
- description: Read release history and the current version
  flows: []
  scope: read:releases
- description: Read documentation pages and run searches
  flows: []
  scope: read:docs
- description: Read pricing and plan data
  flows: []
  scope: read:pricing
- description: Read frequently asked questions
  flows: []
  scope: read:faq
- description: Start and poll documentation export jobs
  flows: []
  scope: export:docs
slug: yappy-biz-scopes
source_filename: yappy-biz-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://yappy.biz/developers/authentication.md\nscopes:\n  - name: read:releases\n    description: \"Read release history and the current version\"\n  - name: read:docs\n    description: \"Read documentation pages and run searches\"\n  - name: read:pricing\n    description: \"Read pricing and plan data\"\n  - name: read:faq\n    description: \"Read frequently asked questions\"\n  - name: export:docs\n    description: \"Start and poll documentation export jobs\"\n"
source_yaml_url: https://artifacts.apis.io/yappy-biz/scopes/yappy-biz-scopes.yml
summary_line: 5 scopes
tags:
- Voice
- macOS
- Automation
- Accessibility
- Productivity
token_bound: false
token_urls: []
---
