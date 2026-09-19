---
api_specs:
- filename: clickup-authorization-api-openapi.yml
  format: yaml
  label: clickup Authorization API
  slug: clickup-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-authorization-api-openapi.yml
- filename: clickup-comments-api-openapi.yml
  format: yaml
  label: clickup Comments API
  slug: clickup-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-comments-api-openapi.yml
- filename: clickup-custom-fields-api-openapi.yml
  format: yaml
  label: clickup Custom Fields API
  slug: clickup-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-custom-fields-api-openapi.yml
- filename: clickup-folders-api-openapi.yml
  format: yaml
  label: clickup Folders API
  slug: clickup-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-folders-api-openapi.yml
- filename: clickup-goals-api-openapi.yml
  format: yaml
  label: clickup Goals API
  slug: clickup-goals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-goals-api-openapi.yml
- filename: clickup-lists-api-openapi.yml
  format: yaml
  label: clickup Lists API
  slug: clickup-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-lists-api-openapi.yml
- filename: clickup-spaces-api-openapi.yml
  format: yaml
  label: clickup Spaces API
  slug: clickup-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-spaces-api-openapi.yml
- filename: clickup-tasks-api-openapi.yml
  format: yaml
  label: clickup Tasks API
  slug: clickup-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-tasks-api-openapi.yml
- filename: clickup-teams-api-openapi.yml
  format: yaml
  label: clickup Teams API
  slug: clickup-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-teams-api-openapi.yml
- filename: clickup-time-tracking-api-openapi.yml
  format: yaml
  label: clickup Time Tracking API
  slug: clickup-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-time-tracking-api-openapi.yml
- filename: clickup-views-api-openapi.yml
  format: yaml
  label: clickup Views API
  slug: clickup-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-views-api-openapi.yml
- filename: clickup-webhooks-api-openapi.yml
  format: yaml
  label: clickup Webhooks API
  slug: clickup-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-webhooks-api-openapi.yml
- filename: clickup-oauth-api-openapi.yml
  format: yaml
  label: Clickup O Auth API
  slug: clickup-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-oauth-api-openapi.yml
- filename: clickup-api-v2-reference-openapi.json
  format: json
  label: ClickUp API v2
  slug: clickup-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-api-v2-reference-openapi.json
- filename: clickup-public-api-v3-openapi.json
  format: json
  label: ClickUp Public API v3
  slug: clickup-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/openapi/clickup-public-api-v3-openapi.json
authorization_urls: []
description: ''
docs: https://developer.clickup.com/docs/authentication
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Clickup Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Clickup publishes 2 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Clickup API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Clickup
provider_slug: clickup
schemes:
- authorization_unit: workspace
  authorization_url: https://app.clickup.com/api
  grant_types:
  - authorization_code
  name: ClickUp OAuth 2.0 (public API)
  note: Access tokens do not expire (documented in the developer FAQ).
  scopes_supported: []
  token_url: https://api.clickup.com/api/v2/oauth/token
- authorization_url: https://mcp.clickup.com/oauth/authorize
  code_challenge_methods:
  - S256
  grant_types:
  - authorization_code
  name: ClickUp MCP server
  registration_url: https://mcp.clickup.com/oauth/register
  source: https://mcp.clickup.com/.well-known/oauth-authorization-server
  token_url: https://mcp.clickup.com/oauth/token
scope_count: 2
scope_names:
- read
- write
scopes:
- description: Read access to the ClickUp MCP resource (tasks, documents, chat).
  flows:
  - authorizationCode
  scope: read
- description: Write access to the ClickUp MCP resource (tasks, documents, chat).
  flows:
  - authorizationCode
  scope: write
slug: clickup-scopes
source_filename: clickup-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  https://developer.clickup.com/docs/authentication and\n  well-known/clickup-mcp-oauth-authorization-server.json\ndocs: https://developer.clickup.com/docs/authentication\nfinding: >-\n  The ClickUp public API OAuth flow has NO scope parameter and NO scope reference page. Authorization is\n  granted per WORKSPACE, not per permission: the user picks which Workspaces an app may access, and the\n  resulting token carries whatever that user can do. Neither published OpenAPI declares an oauth2\n  securityScheme (both declare a single apiKey Authorization header), so derive-oauth-scopes.py has\n  nothing to read — the absence is the contract, not a harvesting gap. The only scoped surface ClickUp\n  operates is the MCP server, whose RFC 8414 metadata advertises two coarse scopes.\nschemes:\n- name: ClickUp OAuth 2.0 (public API)\n  authorization_url: https://app.clickup.com/api\n  token_url: https://api.clickup.com/api/v2/oauth/token\n\
  \  grant_types: [authorization_code]\n  scopes_supported: []\n  authorization_unit: workspace\n  note: Access tokens do not expire (documented in the developer FAQ).\n- name: ClickUp MCP server\n  source: https://mcp.clickup.com/.well-known/oauth-authorization-server\n  authorization_url: https://mcp.clickup.com/oauth/authorize\n  token_url: https://mcp.clickup.com/oauth/token\n  registration_url: https://mcp.clickup.com/oauth/register\n  grant_types: [authorization_code]\n  code_challenge_methods: [S256]\nscopes:\n- scope: read\n  description: Read access to the ClickUp MCP resource (tasks, documents, chat).\n  flows: [authorizationCode]\n  sources: [well-known/clickup-mcp-oauth-authorization-server.json, well-known/clickup-mcp-oauth-protected-resource.json]\n  surface: mcp\n- scope: write\n  description: Write access to the ClickUp MCP resource (tasks, documents, chat).\n  flows: [authorizationCode]\n  sources: [well-known/clickup-mcp-oauth-authorization-server.json, well-known/clickup-mcp-oauth-protected-resource.json]\n\
  \  surface: mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickup/refs/heads/main/scopes/clickup-scopes.yml
summary_line: 2 scopes
tags:
- Project Management
- Work Management
- Productivity
- Collaboration
- Task
- Documents
- Chat
- Time Tracking
- MCP
token_urls: []
---
