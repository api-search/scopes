---
api_specs:
- filename: fastgstrefund-com-checklist-api-openapi.yml
  format: yaml
  label: Fast GST Refund Checklist API
  slug: fastgstrefund-com-checklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastgstrefund-com/openapi/fastgstrefund-com-checklist-api-openapi.yml
- filename: fastgstrefund-com-generator-files-api-openapi.yml
  format: yaml
  label: Fast GST Refund Generator Files API
  slug: fastgstrefund-com-generator-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastgstrefund-com/openapi/fastgstrefund-com-generator-files-api-openapi.yml
- filename: fastgstrefund-com-generators-api-openapi.yml
  format: yaml
  label: Fast GST Refund Generators API
  slug: fastgstrefund-com-generators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fastgstrefund-com/openapi/fastgstrefund-com-generators-api-openapi.yml
authorization_urls:
- https://fastgstrefund.com/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Fastgstrefund Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Fast GST Refund publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Fast GST Refund API on a user''s behalf.


  Tokens are issued from https://fastgstrefund.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Fast GST Refund
provider_slug: fastgstrefund-com
schemes:
- description: OAuth 2.1 authorization code with S256 PKCE. Clients register at /oauth/register. The person signs in with an emailed code. See /.well-known/oauth-authorization-server.
  flows:
  - authorizationUrl: https://fastgstrefund.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://fastgstrefund.com/oauth/token
  name: account
  source: openapi/fastgstrefund-com-openapi.json
- description: OAuth 2.1 authorization code with S256 PKCE. Clients register at /oauth/register. The person signs in with an emailed code. See /.well-known/oauth-authorization-server.
  flows:
  - authorizationUrl: https://fastgstrefund.com/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://fastgstrefund.com/oauth/token
  name: account
  source: openapi/fastgstrefund-com-openapi.yml
scope_count: 1
scope_names:
- refund:generate
scopes:
- description: Check records, and create and download files for claims the account has paid for.
  flows:
  - authorizationCode
  scope: refund:generate
slug: fastgstrefund-com-scopes
source_filename: fastgstrefund-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fastgstrefund-com-openapi.json, openapi/fastgstrefund-com-openapi.yml\nschemes:\n- name: account\n  source: openapi/fastgstrefund-com-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fastgstrefund.com/oauth/authorize\n    tokenUrl: https://fastgstrefund.com/oauth/token\n  description: OAuth 2.1 authorization code with S256 PKCE. Clients register at /oauth/register.\n    The person signs in with an emailed code. See /.well-known/oauth-authorization-server.\n- name: account\n  source: openapi/fastgstrefund-com-openapi.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fastgstrefund.com/oauth/authorize\n    tokenUrl: https://fastgstrefund.com/oauth/token\n  description: OAuth 2.1 authorization code with S256 PKCE. Clients register at /oauth/register.\n    The person signs in with an emailed code. See /.well-known/oauth-authorization-server.\nscopes:\n- scope: refund:generate\n\
  \  description: Check records, and create and download files for claims the account has paid\n    for.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/fastgstrefund-com-openapi.json\n  - openapi/fastgstrefund-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/fastgstrefund-com/scopes/fastgstrefund-com-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- GST refund
- JSON generator
- Exporters
- Chartered accountants
- SaaS companies
- Accounting practices
token_bound: false
token_urls:
- https://fastgstrefund.com/oauth/token
---
