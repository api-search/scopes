---
api_specs:
- filename: craaft-io-attachments-api-openapi.yml
  format: yaml
  label: craaft Attachments API
  slug: craaft-io-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-attachments-api-openapi.yml
- filename: craaft-io-board-templates-api-openapi.yml
  format: yaml
  label: craaft Board Templates API
  slug: craaft-io-board-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-board-templates-api-openapi.yml
- filename: craaft-io-cards-api-openapi.yml
  format: yaml
  label: craaft Cards API
  slug: craaft-io-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-cards-api-openapi.yml
- filename: craaft-io-checklist-api-openapi.yml
  format: yaml
  label: craaft Checklist API
  slug: craaft-io-checklist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-checklist-api-openapi.yml
- filename: craaft-io-columns-api-openapi.yml
  format: yaml
  label: craaft Columns API
  slug: craaft-io-columns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-columns-api-openapi.yml
- filename: craaft-io-comments-api-openapi.yml
  format: yaml
  label: craaft Comments API
  slug: craaft-io-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-comments-api-openapi.yml
- filename: craaft-io-imports-api-openapi.yml
  format: yaml
  label: craaft Imports API
  slug: craaft-io-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-imports-api-openapi.yml
- filename: craaft-io-invitations-api-openapi.yml
  format: yaml
  label: craaft Invitations API
  slug: craaft-io-invitations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-invitations-api-openapi.yml
- filename: craaft-io-me-api-openapi.yml
  format: yaml
  label: craaft Me API
  slug: craaft-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-me-api-openapi.yml
- filename: craaft-io-members-api-openapi.yml
  format: yaml
  label: craaft Members API
  slug: craaft-io-members-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-members-api-openapi.yml
- filename: craaft-io-milestones-api-openapi.yml
  format: yaml
  label: craaft Milestones API
  slug: craaft-io-milestones-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-milestones-api-openapi.yml
- filename: craaft-io-projects-api-openapi.yml
  format: yaml
  label: craaft Projects API
  slug: craaft-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-projects-api-openapi.yml
- filename: craaft-io-public-api-openapi.yml
  format: yaml
  label: craaft Public API
  slug: craaft-io-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-public-api-openapi.yml
- filename: craaft-io-search-api-openapi.yml
  format: yaml
  label: craaft Search API
  slug: craaft-io-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-search-api-openapi.yml
- filename: craaft-io-users-api-openapi.yml
  format: yaml
  label: craaft Users API
  slug: craaft-io-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-users-api-openapi.yml
- filename: craaft-io-version-api-openapi.yml
  format: yaml
  label: craaft Version API
  slug: craaft-io-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-version-api-openapi.yml
- filename: craaft-io-webhooks-api-openapi.yml
  format: yaml
  label: craaft Webhooks API
  slug: craaft-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craaft-io/openapi/craaft-io-webhooks-api-openapi.yml
authorization_urls: []
description: ''
docs: https://craaft.io/docs
flows: []
kind: oauth-scopes
layout: scope
method: searched
name: craaft Scopes
name_suffix: OAuth Scopes
note: The spec declares no oauth2 securityScheme; OAuth 2.1 (authorization code + PKCE) is documented in the bearerAuth description and on https://craaft.io/mcp. The only named scope is craaft:read. The REST guide states "There is no separate scope system"; token restriction is otherwise by access (read / read-write) and by chosen boards.
overview: 'craaft publishes 1 OAuth 2.0 scope. Scopes are the fine-grained permissions an application requests at authorization time to act against the craaft API on a user''s behalf.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: craaft
provider_slug: craaft-io
schemes: []
scope_count: 1
scope_names:
- craaft:read
scopes:
- description: Read-only OAuth grant. A read-only token can send GET, HEAD and OPTIONS; any other method gets 403 "this token is read-only; this request needs a token with read and write access".
  flows: []
  scope: craaft:read
slug: craaft-io-scopes
source_filename: craaft-io-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: openapi/craaft-io-openapi.yml\ndocs: https://craaft.io/docs\nnote: The spec declares no oauth2 securityScheme; OAuth 2.1 (authorization code + PKCE) is documented in the bearerAuth description and on https://craaft.io/mcp. The only named scope is craaft:read. The REST guide states \"There is no separate scope system\"; token restriction is otherwise by access (read / read-write) and by chosen boards.\nscopes:\n- name: craaft:read\n  description: Read-only OAuth grant. A read-only token can send GET, HEAD and OPTIONS; any other method gets 403 \"this token is read-only; this request needs a token with read and write access\".\n  source: openapi/craaft-io-openapi.yml#/components/securitySchemes/bearerAuth\n"
source_yaml_url: https://artifacts.apis.io/craaft-io/scopes/craaft-io-scopes.yml
summary_line: 1 scope
tags:
- Company
- Task Management
- Kanban
- Project Management
- Productivity
- AI Agents
- MCP
- REST API
- Collaboration
token_bound: false
token_urls: []
---
