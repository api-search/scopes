---
api_specs:
- filename: docrocket-ai-brand-from-url-api-openapi.yml
  format: yaml
  label: docrocket-ai Brand From Url API
  slug: docrocket-ai-brand-from-url-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-brand-from-url-api-openapi.yml
- filename: docrocket-ai-generate-document-api-openapi.yml
  format: yaml
  label: docrocket-ai Generate Document API
  slug: docrocket-ai-generate-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-generate-document-api-openapi.yml
- filename: docrocket-ai-get-document-api-openapi.yml
  format: yaml
  label: docrocket-ai Get Document API
  slug: docrocket-ai-get-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-get-document-api-openapi.yml
- filename: docrocket-ai-https-json-api-api-openapi.yml
  format: yaml
  label: docrocket-ai HTTPS JSON API
  slug: docrocket-ai-https-json-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-https-json-api-api-openapi.yml
- filename: docrocket-ai-list-brands-api-openapi.yml
  format: yaml
  label: docrocket-ai List Brands API
  slug: docrocket-ai-list-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-list-brands-api-openapi.yml
- filename: docrocket-ai-list-components-api-openapi.yml
  format: yaml
  label: docrocket-ai List Components API
  slug: docrocket-ai-list-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-list-components-api-openapi.yml
- filename: docrocket-ai-list-templates-api-openapi.yml
  format: yaml
  label: docrocket-ai List Templates API
  slug: docrocket-ai-list-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-list-templates-api-openapi.yml
authorization_urls:
- https://app.docrocket.ai/oauth/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Docrocket Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'docrocket-ai publishes 5 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the docrocket-ai API on a user''s behalf.


  Tokens are issued from https://app.docrocket.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: docrocket-ai
provider_slug: docrocket-ai
schemes:
- description: OAuth 2.0 via DocRocket account. No API keys needed.
  flows:
  - authorizationUrl: https://app.docrocket.ai/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.docrocket.ai/oauth/token
  name: oauth2
  source: openapi/docrocket-ai-openapi.json
scope_count: 5
scope_names:
- brands:read
- brands:write
- documents:read
- documents:write
- templates:read
scopes:
- description: Read brands
  flows:
  - authorizationCode
  scope: brands:read
- description: Create and update brands
  flows:
  - authorizationCode
  scope: brands:write
- description: Read documents
  flows:
  - authorizationCode
  scope: documents:read
- description: Generate documents
  flows:
  - authorizationCode
  scope: documents:write
- description: Read templates
  flows:
  - authorizationCode
  scope: templates:read
slug: docrocket-ai-scopes
source_filename: docrocket-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/docrocket-ai-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/docrocket-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.docrocket.ai/oauth/authorize\n    tokenUrl: https://app.docrocket.ai/oauth/token\n  description: OAuth 2.0 via DocRocket account. No API keys needed.\nscopes:\n- scope: brands:read\n  description: Read brands\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docrocket-ai-openapi.json\n- scope: brands:write\n  description: Create and update brands\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docrocket-ai-openapi.json\n- scope: documents:read\n  description: Read documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docrocket-ai-openapi.json\n- scope: documents:write\n  description: Generate documents\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docrocket-ai-openapi.json\n- scope: templates:read\n  description:\
  \ Read templates\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/docrocket-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/docrocket-ai/scopes/docrocket-ai-scopes.yml
summary_line: 5 scopes · authorizationCode
tags:
- Document Generation
- Multi-tenant SaaS
- Brand Extraction
- PDF Generation
- AI Agents
- MCP Protocol
- SaaS Integration
token_bound: false
token_urls:
- https://app.docrocket.ai/oauth/token
---
