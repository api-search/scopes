---
api_specs:
- filename: syntheticbrew-ai-getting-started-openapi-generated.yml
  format: yaml
  label: SyntheticBrew getting started API
  slug: getting-started-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syntheticbrew-ai/openapi/_ae-authored/syntheticbrew-ai-getting-started-openapi-generated.yml
- filename: syntheticbrew-ai-integration-openapi-generated.yml
  format: yaml
  label: SyntheticBrew integration API
  slug: integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syntheticbrew-ai/openapi/_ae-authored/syntheticbrew-ai-integration-openapi-generated.yml
authorization_urls:
- https://app.syntheticbrew.ai/admin/oauth/consent
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: SyntheticBrew Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'SyntheticBrew publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the SyntheticBrew API on a user''s behalf.


  Tokens are issued from https://app.syntheticbrew.ai/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: SyntheticBrew
provider_slug: syntheticbrew-ai
schemes:
- flows:
  - authorizationUrl: https://app.syntheticbrew.ai/admin/oauth/consent
    flow: authorizationCode
    tokenUrl: https://app.syntheticbrew.ai/oauth/token
  name: MCP_OAuth
  source: openapi/syntheticbrew-ai-getting-started-openapi-generated.yml
- flows:
  - authorizationUrl: https://app.syntheticbrew.ai/admin/oauth/consent
    flow: authorizationCode
    tokenUrl: https://app.syntheticbrew.ai/oauth/token
  name: MCP_OAuth
  source: openapi/syntheticbrew-ai-integration-openapi-generated.yml
- flows:
  - authorizationUrl: https://app.syntheticbrew.ai/admin/oauth/consent
    flow: authorizationCode
    tokenUrl: https://app.syntheticbrew.ai/oauth/token
  name: MCP_OAuth
  source: openapi/syntheticbrew-ai-openapi-generated.yml
scope_count: 3
scope_names:
- manage
- offline_access
- provision
scopes:
- description: ''
  flows:
  - authorizationCode
  scope: manage
- description: ''
  flows:
  - authorizationCode
  scope: offline_access
- description: ''
  flows:
  - authorizationCode
  scope: provision
slug: syntheticbrew-ai-scopes
source_filename: syntheticbrew-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: derived\nsource: openapi/syntheticbrew-ai-getting-started-openapi-generated.yml, openapi/syntheticbrew-ai-integration-openapi-generated.yml,\n  openapi/syntheticbrew-ai-openapi-generated.yml\nschemes:\n- name: MCP_OAuth\n  source: openapi/syntheticbrew-ai-getting-started-openapi-generated.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.syntheticbrew.ai/admin/oauth/consent\n    tokenUrl: https://app.syntheticbrew.ai/oauth/token\n- name: MCP_OAuth\n  source: openapi/syntheticbrew-ai-integration-openapi-generated.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.syntheticbrew.ai/admin/oauth/consent\n    tokenUrl: https://app.syntheticbrew.ai/oauth/token\n- name: MCP_OAuth\n  source: openapi/syntheticbrew-ai-openapi-generated.yml\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.syntheticbrew.ai/admin/oauth/consent\n    tokenUrl: https://app.syntheticbrew.ai/oauth/token\n\
  scopes:\n- scope: manage\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/syntheticbrew-ai-getting-started-openapi-generated.yml\n  - openapi/syntheticbrew-ai-integration-openapi-generated.yml\n  - openapi/syntheticbrew-ai-openapi-generated.yml\n- scope: offline_access\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/syntheticbrew-ai-getting-started-openapi-generated.yml\n  - openapi/syntheticbrew-ai-integration-openapi-generated.yml\n  - openapi/syntheticbrew-ai-openapi-generated.yml\n- scope: provision\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/syntheticbrew-ai-getting-started-openapi-generated.yml\n  - openapi/syntheticbrew-ai-integration-openapi-generated.yml\n  - openapi/syntheticbrew-ai-openapi-generated.yml\n"
source_yaml_url: https://artifacts.apis.io/syntheticbrew-ai/scopes/syntheticbrew-ai-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- AI
- Infrastructure
- Enterprise
- Agents
- NoCode
token_bound: false
token_urls:
- https://app.syntheticbrew.ai/oauth/token
---
