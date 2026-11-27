---
api_specs:
- filename: createya-ai-balance-api-openapi.yml
  format: yaml
  label: Createya Balance API
  slug: createya-ai-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-balance-api-openapi.yml
- filename: createya-ai-healthz-api-openapi.yml
  format: yaml
  label: Createya Healthz API
  slug: createya-ai-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-healthz-api-openapi.yml
- filename: createya-ai-mcp-api-openapi.yml
  format: yaml
  label: Createya MCP API
  slug: createya-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-mcp-api-openapi.yml
- filename: createya-ai-models-api-openapi.yml
  format: yaml
  label: Createya Models API
  slug: createya-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-models-api-openapi.yml
- filename: createya-ai-run-api-openapi.yml
  format: yaml
  label: Createya Run API
  slug: createya-ai-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-run-api-openapi.yml
- filename: createya-ai-runs-api-openapi.yml
  format: yaml
  label: Createya Runs API
  slug: createya-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-runs-api-openapi.yml
- filename: createya-ai-uploads-api-openapi.yml
  format: yaml
  label: Createya Uploads API
  slug: createya-ai-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createya-ai/openapi/createya-ai-uploads-api-openapi.yml
authorization_urls: []
description: ''
docs: https://github.com/Createya-ai/createya-mcp/blob/main/examples/10-error-handling.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Createya Scopes
name_suffix: OAuth Scopes
note: These are API-key scopes, not OAuth scopes in the OpenAPI (which declares only http bearer). The error reference names them in the insufficient_scope remediation; no dedicated scopes page was found on docs.createya.ai.
overview: 'Createya publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Createya API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Createya
provider_slug: createya-ai
schemes: []
scope_count: 2
scope_names:
- generate
- read:usage
scopes:
- description: Scope required to run generations (named in the 403 insufficient_scope remediation).
  flows: []
  scope: generate
- description: Scope for reading usage (named in the 403 insufficient_scope remediation).
  flows: []
  scope: read:usage
slug: createya-ai-scopes
source_filename: createya-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://github.com/Createya-ai/createya-mcp/blob/main/examples/10-error-handling.md\ndocs: https://github.com/Createya-ai/createya-mcp/blob/main/examples/10-error-handling.md\nnote: These are API-key scopes, not OAuth scopes in the OpenAPI (which declares only http bearer). The error reference names them in the insufficient_scope remediation; no dedicated scopes page was found on docs.createya.ai.\nscopes:\n- name: generate\n  description: Scope required to run generations (named in the 403 insufficient_scope remediation).\n- name: read:usage\n  description: Scope for reading usage (named in the 403 insufficient_scope remediation).\n"
source_yaml_url: https://artifacts.apis.io/createya-ai/scopes/createya-ai-scopes.yml
summary_line: 2 scopes
tags:
- Company
- Artificial Intelligence
- Generative AI
- Image Generation
- Video Generation
- Audio Generation
- Model Aggregator
- MCP
token_bound: false
token_urls: []
---
