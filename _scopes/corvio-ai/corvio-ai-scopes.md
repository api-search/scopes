---
api_specs:
- filename: corvio-ai-agent-collaboration-api-openapi.yml
  format: yaml
  label: Corvio Agent collaboration API
  slug: corvio-ai-agent-collaboration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-agent-collaboration-api-openapi.yml
- filename: corvio-ai-public-api-v1-api-openapi.yml
  format: yaml
  label: Corvio Public API v1 API
  slug: corvio-ai-public-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-public-api-v1-api-openapi.yml
- filename: corvio-ai-public-api-v1-files-api-openapi.yml
  format: yaml
  label: Corvio Public API v1 - Files API
  slug: corvio-ai-public-api-v1-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-public-api-v1-files-api-openapi.yml
- filename: corvio-ai-public-api-v1-local-markdown-sync-api-openapi.yml
  format: yaml
  label: Corvio Public API v1 - Local Markdown Sync API
  slug: corvio-ai-public-api-v1-local-markdown-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-public-api-v1-local-markdown-sync-api-openapi.yml
- filename: corvio-ai-public-api-v1-source-publication-api-openapi.yml
  format: yaml
  label: Corvio Public API v1 - Source publication API
  slug: corvio-ai-public-api-v1-source-publication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/corvio-ai/openapi/corvio-ai-public-api-v1-source-publication-api-openapi.yml
authorization_urls: []
description: ''
docs: https://corvio.ai/developers/skills/corvio-operate-workspace/references/api.md
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: Corvio Scopes
name_suffix: OAuth Scopes
note: The REST OpenAPI declares no oauth2 scheme; scopes are documented for API keys and Remote MCP OAuth. Only the scope names the docs name verbatim are listed — the docs say "The live OpenAPI is the HTTP method, path, field, scope, and error authority", but the OpenAPI publishes none.
overview: 'Corvio publishes 5 OAuth 2.0 scopes. Scopes are the fine-grained permissions an application requests at authorization time to act against the Corvio API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Corvio
provider_slug: corvio-ai
schemes: []
scope_count: 5
scope_names:
- questions:write
- documents:write
- comments:read
- comments:write
- admin_content:read
scopes:
- description: Required, with documents:write and document edit authority, for question runs that write documents (api.md).
  flows: []
  scope: questions:write
- description: Document write capability (api.md).
  flows: []
  scope: documents:write
- description: Remote MCP comment list via explicit OAuth scope (api.md).
  flows: []
  scope: comments:read
- description: Remote MCP comment create/reply/status and explicit change_summary discussion comments (api.md).
  flows: []
  scope: comments:write
- description: Admin CLI; "Exact Run content requires an explicit admin_content:read re-authorization." (https://corvio.ai/developers/admin-cli)
  flows: []
  scope: admin_content:read
slug: corvio-ai-scopes
source_filename: corvio-ai-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://corvio.ai/developers/skills/corvio-operate-workspace/references/api.md\ndocs: https://corvio.ai/developers/skills/corvio-operate-workspace/references/api.md\nnote: The REST OpenAPI declares no oauth2 scheme; scopes are documented for API keys and Remote MCP OAuth. Only the scope names the docs name verbatim are listed — the docs say \"The live OpenAPI is the HTTP method, path, field, scope, and error authority\", but the OpenAPI publishes none.\nscopes:\n- name: questions:write\n  description: Required, with documents:write and document edit authority, for question runs that write documents (api.md).\n- name: documents:write\n  description: Document write capability (api.md).\n- name: comments:read\n  description: Remote MCP comment list via explicit OAuth scope (api.md).\n- name: comments:write\n  description: Remote MCP comment create/reply/status and explicit change_summary discussion comments (api.md).\n- name:\
  \ admin_content:read\n  description: Admin CLI; \"Exact Run content requires an explicit admin_content:read re-authorization.\" (https://corvio.ai/developers/admin-cli)\n"
source_yaml_url: https://artifacts.apis.io/corvio-ai/scopes/corvio-ai-scopes.yml
summary_line: 5 scopes
tags:
- Company
- Artificial Intelligence
- Notes
- Knowledge Management
- Workspace
- AI Agents
- MCP
- Developer API
- CLI
token_bound: false
token_urls: []
---
