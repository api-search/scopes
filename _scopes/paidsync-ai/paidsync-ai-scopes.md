---
api_specs:
- filename: paidsync-ai-billing-api-openapi.yml
  format: yaml
  label: paidsync-ai Billing API
  slug: paidsync-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-billing-api-openapi.yml
- filename: paidsync-ai-mcp-api-openapi.yml
  format: yaml
  label: paidsync-ai MCP API
  slug: paidsync-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-mcp-api-openapi.yml
- filename: paidsync-ai-paidsync-api-api-openapi.yml
  format: yaml
  label: paidsync-ai PaidSync API
  slug: paidsync-ai-paidsync-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-paidsync-api-api-openapi.yml
- filename: paidsync-ai-payment-api-openapi.yml
  format: yaml
  label: paidsync-ai Payment API
  slug: paidsync-ai-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-payment-api-openapi.yml
- filename: paidsync-ai-subscribe-api-openapi.yml
  format: yaml
  label: paidsync-ai Subscribe API
  slug: paidsync-ai-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-subscribe-api-openapi.yml
authorization_urls:
- https://api.paidsync.ai/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Paidsync Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'paidsync-ai publishes 4 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the paidsync-ai API on a user''s behalf.


  Tokens are issued from https://api.paidsync.ai/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: paidsync-ai
provider_slug: paidsync-ai
schemes:
- flows:
  - authorizationUrl: https://api.paidsync.ai/authorize
    flow: authorizationCode
    tokenUrl: https://api.paidsync.ai/token
  name: oauth2
  source: openapi/paidsync-ai-openapi.json
scope_count: 4
scope_names:
- ads
- email
- openid
- profile
scopes:
- description: Ad platform access
  flows:
  - authorizationCode
  scope: ads
- description: Email address
  flows:
  - authorizationCode
  scope: email
- description: OpenID identity
  flows:
  - authorizationCode
  scope: openid
- description: Basic profile
  flows:
  - authorizationCode
  scope: profile
slug: paidsync-ai-scopes
source_filename: paidsync-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/paidsync-ai-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/paidsync-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.paidsync.ai/authorize\n    tokenUrl: https://api.paidsync.ai/token\nscopes:\n- scope: ads\n  description: Ad platform access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/paidsync-ai-openapi.json\n- scope: email\n  description: Email address\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/paidsync-ai-openapi.json\n- scope: openid\n  description: OpenID identity\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/paidsync-ai-openapi.json\n- scope: profile\n  description: Basic profile\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/paidsync-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/paidsync-ai/scopes/paidsync-ai-scopes.yml
summary_line: 4 scopes · authorizationCode
tags:
- Company
- AI
- Advertising
- Automation
- Marketing
token_bound: false
token_urls:
- https://api.paidsync.ai/token
---
