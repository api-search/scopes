---
api_specs:
- filename: pipedream-openapi.yml
  format: yaml
  label: Pipedream REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-openapi.yml
- filename: pipedream-openapi.yml
  format: yaml
  label: Pipedream Connect
  slug: connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-openapi.yml
- filename: pipedream-mcp-openapi.yml
  format: yaml
  label: Pipedream MCP Server
  slug: mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/openapi/pipedream-mcp-openapi.yml
authorization_urls: []
description: ''
docs: ''
flows:
- clientCredentials
kind: oauth-scopes
layout: scope
method: derived
name: Pipedream Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Pipedream publishes 16 OAuth 2.0 scopes via the clientCredentials flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Pipedream API on a user''s behalf.


  Tokens are issued from https://api.pipedream.com/v1/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Pipedream
provider_slug: pipedream
schemes:
- description: A short-lived OAuth access token for server-side requests. Generate one via the Generate OAuth Token flow or automatically when initializing the SDK client.
  flows:
  - flow: clientCredentials
    tokenUrl: https://api.pipedream.com/v1/oauth/token
  name: OAuth2
  source: openapi/pipedream-openapi.yml
scope_count: 16
scope_names:
- '*'
- connect:*
- connect:accounts:read
- connect:accounts:write
- connect:actions:*
- connect:deployed_triggers:read
- connect:deployed_triggers:write
- connect:projects:read
- connect:projects:write
- connect:proxy
- connect:tokens:create
- connect:triggers:*
- connect:usage:read
- connect:users:read
- connect:users:write
- connect:workflow:invoke
scopes:
- description: Full access to every OAuth-protected endpoint.
  flows:
  - clientCredentials
  scope: '*'
- description: Full access to all Connect API endpoints (components, projects, triggers, accounts, etc.).
  flows:
  - clientCredentials
  scope: connect:*
- description: List and fetch Connect accounts for an external user.
  flows:
  - clientCredentials
  scope: connect:accounts:read
- description: Create or remove Connect accounts.
  flows:
  - clientCredentials
  scope: connect:accounts:write
- description: Full access to Connect actions.
  flows:
  - clientCredentials
  scope: connect:actions:*
- description: Read deployed triggers and related data like events, pipelines and webhooks.
  flows:
  - clientCredentials
  scope: connect:deployed_triggers:read
- description: Modify or delete deployed triggers.
  flows:
  - clientCredentials
  scope: connect:deployed_triggers:write
- description: List and fetch projects owned by the workspace.
  flows:
  - clientCredentials
  scope: connect:projects:read
- description: Create, update, or delete projects owned by the workspace.
  flows:
  - clientCredentials
  scope: connect:projects:write
- description: Invoke the Connect proxy.
  flows:
  - clientCredentials
  scope: connect:proxy
- description: Create Connect session tokens.
  flows:
  - clientCredentials
  scope: connect:tokens:create
- description: Full access to Connect triggers.
  flows:
  - clientCredentials
  scope: connect:triggers:*
- description: List Connect usage records for a time window.
  flows:
  - clientCredentials
  scope: connect:usage:read
- description: List and fetch external users
  flows:
  - clientCredentials
  scope: connect:users:read
- description: Delete external users.
  flows:
  - clientCredentials
  scope: connect:users:write
- description: Invoke Connect workflows on behalf of a user.
  flows:
  - clientCredentials
  scope: connect:workflow:invoke
slug: pipedream-scopes
source_filename: pipedream-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pipedream-openapi.yml\nschemes:\n- name: OAuth2\n  source: openapi/pipedream-openapi.yml\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.pipedream.com/v1/oauth/token\n  description: A short-lived OAuth access token for server-side requests. Generate one via the\n    Generate OAuth Token flow or automatically when initializing the SDK client.\nscopes:\n- scope: '*'\n  description: Full access to every OAuth-protected endpoint.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:*\n  description: Full access to all Connect API endpoints (components, projects, triggers, accounts,\n    etc.).\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:accounts:read\n  description: List and fetch Connect accounts for an external user.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope:\
  \ connect:accounts:write\n  description: Create or remove Connect accounts.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:actions:*\n  description: Full access to Connect actions.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:deployed_triggers:read\n  description: Read deployed triggers and related data like events, pipelines and webhooks.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:deployed_triggers:write\n  description: Modify or delete deployed triggers.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:projects:read\n  description: List and fetch projects owned by the workspace.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:projects:write\n  description: Create, update, or delete projects owned by the workspace.\n  flows:\n  - clientCredentials\n\
  \  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:proxy\n  description: Invoke the Connect proxy.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:tokens:create\n  description: Create Connect session tokens.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:triggers:*\n  description: Full access to Connect triggers.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:usage:read\n  description: List Connect usage records for a time window.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:users:read\n  description: List and fetch external users\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:users:write\n  description: Delete external users.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n- scope: connect:workflow:invoke\n\
  \  description: Invoke Connect workflows on behalf of a user.\n  flows:\n  - clientCredentials\n  sources:\n  - openapi/pipedream-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pipedream/refs/heads/main/scopes/pipedream-scopes.yml
summary_line: 16 scopes · clientCredentials
tags:
- ProCode_API_Composition
- Workflows
- Connect
- MCP
- Embedded Integrations
- Managed Auth
- AI Agents
token_urls:
- https://api.pipedream.com/v1/oauth/token
---
