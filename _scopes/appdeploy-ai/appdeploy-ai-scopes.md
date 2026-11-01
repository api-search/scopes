---
api_specs:
- filename: appdeploy-ai-mcp-api-openapi.yml
  format: yaml
  label: appdeploy-ai MCP API
  slug: appdeploy-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appdeploy-ai/openapi/appdeploy-ai-mcp-api-openapi.yml
- filename: appdeploy-ai-oauth-discovery-api-openapi.yml
  format: yaml
  label: appdeploy-ai OAuth discovery API
  slug: appdeploy-ai-oauth-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/appdeploy-ai/openapi/appdeploy-ai-oauth-discovery-api-openapi.yml
authorization_urls:
- https://api-v2.appdeploy.ai/mcp/authorize
description: ''
docs: ''
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: derived
name: Appdeploy Ai Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'appdeploy-ai publishes 3 OAuth 2.0 scopes via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the appdeploy-ai API on a user''s behalf.


  Tokens are issued from https://api-v2.appdeploy.ai/mcp/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: appdeploy-ai
provider_slug: appdeploy-ai
schemes:
- description: OAuth 2.0 Authorization Code flow with PKCE and dynamic client registration. AppDeploy declares separate tool permission scopes for read, write, and delete operations.
  flows:
  - authorizationUrl: https://api-v2.appdeploy.ai/mcp/authorize
    flow: authorizationCode
    tokenUrl: https://api-v2.appdeploy.ai/mcp/token
  name: AppDeployOAuth
  source: openapi/appdeploy-ai-openapi.json
scope_count: 3
scope_names:
- deploy:delete
- deploy:read
- deploy:write
scopes:
- description: Delete an app. Intended only for an explicit destructive delete operation.
  flows:
  - authorizationCode
  scope: deploy:delete
- description: Read deployment instructions and SDK reference; list and inspect apps, deployment status, versions, logs, and source.
  flows:
  - authorizationCode
  scope: deploy:read
- description: Create or update app deployments, apply versions, and change app configuration.
  flows:
  - authorizationCode
  scope: deploy:write
slug: appdeploy-ai-scopes
source_filename: appdeploy-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: openapi/appdeploy-ai-openapi.json\nschemes:\n- name: AppDeployOAuth\n  source: openapi/appdeploy-ai-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api-v2.appdeploy.ai/mcp/authorize\n    tokenUrl: https://api-v2.appdeploy.ai/mcp/token\n  description: OAuth 2.0 Authorization Code flow with PKCE and dynamic client registration.\n    AppDeploy declares separate tool permission scopes for read, write, and delete operations.\nscopes:\n- scope: deploy:delete\n  description: Delete an app. Intended only for an explicit destructive delete operation.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/appdeploy-ai-openapi.json\n- scope: deploy:read\n  description: Read deployment instructions and SDK reference; list and inspect apps, deployment\n    status, versions, logs, and source.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/appdeploy-ai-openapi.json\n- scope: deploy:write\n \
  \ description: Create or update app deployments, apply versions, and change app configuration.\n  flows:\n  - authorizationCode\n  sources:\n  - openapi/appdeploy-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/appdeploy-ai/scopes/appdeploy-ai-scopes.yml
summary_line: 3 scopes · authorizationCode
tags:
- Company
- AI
- Deployment
- Platform
- LowCode
- Automation
token_bound: false
token_urls:
- https://api-v2.appdeploy.ai/mcp/token
---
