---
api_specs:
- filename: code-ocean-openapi.yml
  format: yaml
  label: Code Ocean API
  slug: code-ocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/code-ocean/refs/heads/main/openapi/code-ocean-openapi.yml
authorization_urls: []
description: ''
docs: https://docs.codeocean.com/user-guide/code-ocean-api/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Code Ocean Scopes
name_suffix: OAuth Scopes
note: Code Ocean authenticates with scoped personal access tokens (prefix cop_) presented via HTTP Basic auth — not an OAuth2 authorization flow. Each token is minted with per-resource permission scopes selected in the Access Tokens UI (Account -> Access Tokens -> Generate New Token -> Select Scopes). The scopes below are the resource permissions documented as API prerequisites; the full enumerated list in the token UI is not published on a single docs page.
overview: 'Code Ocean publishes 4 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Code Ocean API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Code Ocean
provider_slug: code-ocean
schemes:
- name: accessToken
  source: openapi/code-ocean-openapi.yml
  transport: http-basic
  type: personal-access-token
scope_count: 4
scope_names:
- Capsule - Read
- Capsule - Write
- Data Asset - Read
- Data Asset - Write
scopes:
- description: Get capsule, list capsule computations, get app panel.
  flows: []
  scope: Capsule - Read
- description: Delete archived capsule/pipeline, archive/unarchive capsule.
  flows: []
  scope: Capsule - Write
- description: Get data asset, list data asset files, generate file URLs.
  flows: []
  scope: Data Asset - Read
- description: Create, update, archive, and delete data assets.
  flows: []
  scope: Data Asset - Write
slug: code-ocean-scopes
source_filename: code-ocean-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/code-ocean-openapi.yml\ndocs: https://docs.codeocean.com/user-guide/code-ocean-api/authentication\nnote: >-\n  Code Ocean authenticates with scoped personal access tokens (prefix cop_)\n  presented via HTTP Basic auth — not an OAuth2 authorization flow. Each token\n  is minted with per-resource permission scopes selected in the Access Tokens\n  UI (Account -> Access Tokens -> Generate New Token -> Select Scopes). The\n  scopes below are the resource permissions documented as API prerequisites;\n  the full enumerated list in the token UI is not published on a single docs\n  page.\nschemes:\n- name: accessToken\n  type: personal-access-token\n  transport: http-basic\n  source: openapi/code-ocean-openapi.yml\nscopes:\n- scope: Capsule - Read\n  description: Get capsule, list capsule computations, get app panel.\n  sources: [https://docs.codeocean.com/user-guide/code-ocean-api]\n- scope: Capsule - Write\n  description:\
  \ Delete archived capsule/pipeline, archive/unarchive capsule.\n  sources: [https://docs.codeocean.com/user-guide/code-ocean-api]\n- scope: Data Asset - Read\n  description: Get data asset, list data asset files, generate file URLs.\n  sources: [https://docs.codeocean.com/user-guide/code-ocean-api]\n- scope: Data Asset - Write\n  description: Create, update, archive, and delete data assets.\n  sources: [https://docs.codeocean.com/user-guide/code-ocean-api]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/code-ocean/refs/heads/main/scopes/code-ocean-scopes.yml
summary_line: 4 scopes
tags:
- Company
- Reproducible Research
- Computational Science
- Data Science
- Research Computing
- Life Sciences
- Pipelines
- MLOps
- Cloud Platform
- Developer Tools
token_urls: []
---
