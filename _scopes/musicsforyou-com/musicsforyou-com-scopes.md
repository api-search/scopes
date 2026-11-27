---
api_specs:
- filename: musicsforyou-com-account-api-openapi.yml
  format: yaml
  label: 桃源 Account API
  slug: musicsforyou-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-account-api-openapi.yml
- filename: musicsforyou-com-billing-api-openapi.yml
  format: yaml
  label: 桃源 Billing API
  slug: musicsforyou-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-billing-api-openapi.yml
- filename: musicsforyou-com-catalog-api-openapi.yml
  format: yaml
  label: 桃源 Catalog API
  slug: musicsforyou-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-catalog-api-openapi.yml
- filename: musicsforyou-com-compose-api-openapi.yml
  format: yaml
  label: 桃源 Compose API
  slug: musicsforyou-com-compose-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-compose-api-openapi.yml
- filename: musicsforyou-com-edit-api-openapi.yml
  format: yaml
  label: 桃源 Edit API
  slug: musicsforyou-com-edit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-edit-api-openapi.yml
- filename: musicsforyou-com-generate-api-openapi.yml
  format: yaml
  label: 桃源 Generate API
  slug: musicsforyou-com-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-generate-api-openapi.yml
- filename: musicsforyou-com-keys-api-openapi.yml
  format: yaml
  label: 桃源 Keys API
  slug: musicsforyou-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-keys-api-openapi.yml
- filename: musicsforyou-com-library-api-openapi.yml
  format: yaml
  label: 桃源 Library API
  slug: musicsforyou-com-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/musicsforyou-com/openapi/musicsforyou-com-library-api-openapi.yml
authorization_urls:
- https://www.musicsforyou.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: 桃源 Scopes
name_suffix: OAuth Scopes
note: ''
overview: '桃源 publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the 桃源 API on a user''s behalf.


  Tokens are issued from https://api.musicsforyou.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: 桃源
provider_slug: musicsforyou-com
schemes:
- description: 给 ChatGPT / claude.ai 等连接器用的授权码流程 / Authorization-code flow for connector platforms.
  flows:
  - authorizationUrl: https://www.musicsforyou.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://api.musicsforyou.com/oauth/token
  name: OAuth2
  source: openapi/musicsforyou-com-openapi.json
scope_count: 1
scope_names:
- music
scopes:
- description: 编译、生成、查询作品与额度 / Compile, generate, read tracks and credits
  flows:
  - authorizationCode
  scope: music
slug: musicsforyou-com-scopes
source_filename: musicsforyou-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/musicsforyou-com-openapi.json\nschemes:\n- name: OAuth2\n  source: openapi/musicsforyou-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.musicsforyou.com/oauth/authorize\n    tokenUrl: https://api.musicsforyou.com/oauth/token\n  description: 给 ChatGPT / claude.ai 等连接器用的授权码流程 / Authorization-code flow for connector platforms.\nscopes:\n- scope: music\n  description: 编译、生成、查询作品与额度 / Compile, generate, read tracks and credits\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/musicsforyou-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/musicsforyou-com/scopes/musicsforyou-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Company
token_bound: false
token_urls:
- https://api.musicsforyou.com/oauth/token
---
