---
api_specs:
- filename: intencheck-com-analyze-api-openapi.yml
  format: yaml
  label: intencheck-com Analyze API
  slug: intencheck-com-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-analyze-api-openapi.yml
- filename: intencheck-com-api-keys-api-openapi.yml
  format: yaml
  label: intencheck-com API Keys API
  slug: intencheck-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-api-keys-api-openapi.yml
- filename: intencheck-com-checkout-api-openapi.yml
  format: yaml
  label: intencheck-com Checkout API
  slug: intencheck-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-checkout-api-openapi.yml
- filename: intencheck-com-demo-api-openapi.yml
  format: yaml
  label: intencheck-com Demo API
  slug: intencheck-com-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-demo-api-openapi.yml
- filename: intencheck-com-docs-api-openapi.yml
  format: yaml
  label: intencheck-com Docs API
  slug: intencheck-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-docs-api-openapi.yml
- filename: intencheck-com-mcp-api-openapi.yml
  format: yaml
  label: intencheck-com MCP API
  slug: intencheck-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-mcp-api-openapi.yml
- filename: intencheck-com-reply-api-openapi.yml
  format: yaml
  label: intencheck-com Reply API
  slug: intencheck-com-reply-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-reply-api-openapi.yml
- filename: intencheck-com-report-error-api-openapi.yml
  format: yaml
  label: intencheck-com Report Error API
  slug: intencheck-com-report-error-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-report-error-api-openapi.yml
- filename: intencheck-com-transactions-api-openapi.yml
  format: yaml
  label: intencheck-com Transactions API
  slug: intencheck-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-transactions-api-openapi.yml
- filename: intencheck-com-webhooks-api-openapi.yml
  format: yaml
  label: intencheck-com Webhooks API
  slug: intencheck-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intencheck-com/openapi/intencheck-com-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- password
kind: oauth-scopes
layout: scope
method: none
name: Intencheck Com Scopes
name_suffix: OAuth Scopes
note: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement references one.
overview: 'intencheck-com uses OAuth 2.0 but publishes no discrete scopes — access is governed by the grant itself (e.g. client-credentials or role-based authorization) rather than per-scope consent.


  Tokens are issued from /api/v1/auth/login.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: intencheck-com
provider_slug: intencheck-com
schemes:
- flows:
  - flow: password
    tokenUrl: /api/v1/auth/login
  name: OAuth2PasswordBearer
  source: openapi/intencheck-com-openapi.json
scope_count: 0
scope_names: []
scopes: []
slug: intencheck-com-scopes
source_filename: intencheck-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: none\nsource: openapi/intencheck-com-openapi.json\nschemes:\n- name: OAuth2PasswordBearer\n  source: openapi/intencheck-com-openapi.json\n  flows:\n  - flow: password\n    tokenUrl: /api/v1/auth/login\nscopes: []\nnote: The OAuth2 security scheme(s) in the OpenAPI declare no scopes, and no security requirement\n  references one.\n"
source_yaml_url: https://artifacts.apis.io/intencheck-com/scopes/intencheck-com-scopes.yml
summary_line: OAuth 2.0 · no documented scopes
tags:
- Artificial Intelligence
- Natural Language Processing
- Text Analysis
- Sentiment
- Emotion
token_bound: false
token_urls:
- /api/v1/auth/login
---
