---
api_specs:
- filename: justautomate-ai-agents-api-openapi.yml
  format: yaml
  label: JustAutomate Agents API
  slug: justautomate-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-agents-api-openapi.yml
- filename: justautomate-ai-contact-api-openapi.yml
  format: yaml
  label: JustAutomate Contact API
  slug: justautomate-ai-contact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-contact-api-openapi.yml
- filename: justautomate-ai-content-api-openapi.yml
  format: yaml
  label: JustAutomate Content API
  slug: justautomate-ai-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-content-api-openapi.yml
- filename: justautomate-ai-meta-api-openapi.yml
  format: yaml
  label: JustAutomate Meta API
  slug: justautomate-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-meta-api-openapi.yml
- filename: justautomate-ai-offer-api-openapi.yml
  format: yaml
  label: JustAutomate Offer API
  slug: justautomate-ai-offer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justautomate-ai/openapi/justautomate-ai-offer-api-openapi.yml
authorization_urls:
- https://justautomate.ai/oauth/authorize/
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: JustAutomate Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'JustAutomate publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the JustAutomate API on a user''s behalf.


  Tokens are issued from https://justautomate.ai/oauth/token/.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: JustAutomate
provider_slug: justautomate-ai
schemes:
- description: Optional. Identifies the agent and raises the rate limit to 600 requests per minute. Dynamic client registration and anonymous agent registration are described at https://justautomate.ai/auth.md.
  flows:
  - authorizationUrl: https://justautomate.ai/oauth/authorize/
    flow: authorizationCode
    tokenUrl: https://justautomate.ai/oauth/token/
  name: agentOAuth
  source: openapi/justautomate-ai-openapi.json
scope_count: 1
scope_names:
- mcp:read
scopes:
- description: Read public content of justautomate.ai (REST API and MCP server).
  flows:
  - authorizationCode
  scope: mcp:read
slug: justautomate-ai-scopes
source_filename: justautomate-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/justautomate-ai-openapi.json\nschemes:\n- name: agentOAuth\n  source: openapi/justautomate-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://justautomate.ai/oauth/authorize/\n    tokenUrl: https://justautomate.ai/oauth/token/\n  description: Optional. Identifies the agent and raises the rate limit to 600 requests per\n    minute. Dynamic client registration and anonymous agent registration are described at https://justautomate.ai/auth.md.\nscopes:\n- scope: mcp:read\n  description: Read public content of justautomate.ai (REST API and MCP server).\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/justautomate-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/justautomate-ai/scopes/justautomate-ai-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Artificial Intelligence
- Automation
- B2B
- Process Optimization
- Software-as-a-Service
- Company
token_bound: false
token_urls:
- https://justautomate.ai/oauth/token/
---
