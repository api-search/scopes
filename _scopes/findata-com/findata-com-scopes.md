---
api_specs:
- filename: findata-com-companies-api-openapi.yml
  format: yaml
  label: FinData Companies API
  slug: findata-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findata-com/openapi/findata-com-companies-api-openapi.yml
- filename: findata-com-corporate-actions-api-openapi.yml
  format: yaml
  label: FinData Corporate actions API
  slug: findata-com-corporate-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findata-com/openapi/findata-com-corporate-actions-api-openapi.yml
- filename: findata-com-fundamentals-api-openapi.yml
  format: yaml
  label: FinData Fundamentals API
  slug: findata-com-fundamentals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/findata-com/openapi/findata-com-fundamentals-api-openapi.yml
authorization_urls:
- https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: FinData Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'FinData publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the FinData API on a user''s behalf.


  Tokens are issued from https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: FinData
provider_slug: findata-com
schemes:
- description: Authorization code with PKCE. Include resource=https://api.findata.com in both authorization and token requests.
  flows:
  - authorizationUrl: https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/token
  name: OAuth
  source: openapi/findata-com-openapi.json
scope_count: 1
scope_names:
- openid
scopes:
- description: Identify the registered user
  flows:
  - authorizationCode
  scope: openid
slug: findata-com-scopes
source_filename: findata-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/findata-com-openapi.json\nschemes:\n- name: OAuth\n  source: openapi/findata-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/authorize\n    tokenUrl: https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/token\n  description: Authorization code with PKCE. Include resource=https://api.findata.com in both\n    authorization and token requests.\nscopes:\n- scope: openid\n  description: Identify the registered user\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/findata-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/findata-com/scopes/findata-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Financial Data
- SEC Fundamentals
- Market Data
- Research
token_bound: false
token_urls:
- https://ep-proud-butterfly-beqp77bl.neonauth.c-9.us-east-2.aws.neon.tech/neondb/auth/oauth2/token
---
