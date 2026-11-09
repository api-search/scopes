---
api_specs:
- filename: basecite-com-admin-api-openapi.yml
  format: yaml
  label: BaseCite Admin API
  slug: basecite-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-admin-api-openapi.yml
- filename: basecite-com-ai-api-openapi.yml
  format: yaml
  label: BaseCite AI API
  slug: basecite-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-ai-api-openapi.yml
- filename: basecite-com-oauth-api-openapi.yml
  format: yaml
  label: BaseCite OAuth API
  slug: basecite-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-oauth-api-openapi.yml
- filename: basecite-com-organizations-api-openapi.yml
  format: yaml
  label: BaseCite Organizations API
  slug: basecite-com-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-organizations-api-openapi.yml
- filename: basecite-com-portal-api-openapi.yml
  format: yaml
  label: BaseCite Portal API
  slug: basecite-com-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-portal-api-openapi.yml
- filename: basecite-com-sandbox-api-openapi.yml
  format: yaml
  label: BaseCite Sandbox API
  slug: basecite-com-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/basecite-com/openapi/basecite-com-sandbox-api-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Basecite Com Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'BaseCite publishes 7 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the BaseCite API on a user''s behalf.


  Tokens are issued from https://api.basecite.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: BaseCite
provider_slug: basecite-com
schemes:
- flows:
  - flow: clientCredentials
    tokenUrl: https://api.basecite.com/oauth/token
  name: oauth2
  source: openapi/basecite-com-openapi.json
scope_count: 7
scope_names:
- ai_context
- ai_readiness
- correction
- customer_upload
- mcp
- metadata_read
- origin_cairn_reference
scopes:
- description: Read bounded AI context for the bound organization.
  flows:
  - clientCredentials
  scope: ai_context
- description: Read bounded AI-readiness and processing metadata for the bound organization.
  flows:
  - clientCredentials
  scope: ai_readiness
- description: Create organization-scoped upload corrections.
  flows:
  - clientCredentials
  scope: correction
- description: Create and complete organization-scoped customer uploads.
  flows:
  - clientCredentials
  scope: customer_upload
- description: Use authenticated bounded MCP tools for the bound organization.
  flows:
  - clientCredentials
  scope: mcp
- description: Read metadata and canonical upload status for the bound organization.
  flows:
  - clientCredentials
  scope: metadata_read
- description: Attach organization-scoped OriginCairn references.
  flows:
  - clientCredentials
  scope: origin_cairn_reference
slug: basecite-com-scopes
source_filename: basecite-com-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/basecite-com-openapi.json\nschemes:\n- name: oauth2\n  source: openapi/basecite-com-openapi.json\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.basecite.com/oauth/token\nscopes:\n- scope: ai_context\n  description: Read bounded AI context for the bound organization.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basecite-com-openapi.json\n- scope: ai_readiness\n  description: Read bounded AI-readiness and processing metadata for the bound organization.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basecite-com-openapi.json\n- scope: correction\n  description: Create organization-scoped upload corrections.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basecite-com-openapi.json\n- scope: customer_upload\n  description: Create and complete organization-scoped customer uploads.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basecite-com-openapi.json\n- scope:\
  \ mcp\n  description: Use authenticated bounded MCP tools for the bound organization.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basecite-com-openapi.json\n- scope: metadata_read\n  description: Read metadata and canonical upload status for the bound organization.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basecite-com-openapi.json\n- scope: origin_cairn_reference\n  description: Attach organization-scoped OriginCairn references.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/basecite-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/basecite-com/scopes/basecite-com-scopes.yml
summary_line: 7 scopes · clientCredentials
tags:
- Company
- Artificial Intelligence
- Evidence
- Platform
- Privacy
token_bound: false
token_urls:
- https://api.basecite.com/oauth/token
---
