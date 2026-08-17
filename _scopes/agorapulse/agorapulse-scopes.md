---
api_specs:
- filename: agorapulse-calendar-notes-api-openapi.yml
  format: yaml
  label: Agorapulse Calendar Notes API
  slug: agorapulse-calendar-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-calendar-notes-api-openapi.yml
- filename: agorapulse-agorapulse-api-api-openapi.yml
  format: yaml
  label: Agorapulse Webhooks API
  slug: agorapulse-agorapulse-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-agorapulse-api-api-openapi.yml
- filename: agorapulse-competitor-api-openapi.yml
  format: yaml
  label: Agorapulse Competitor API
  slug: agorapulse-competitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-competitor-api-openapi.yml
- filename: agorapulse-conversations-api-openapi.yml
  format: yaml
  label: Agorapulse Conversations API
  slug: agorapulse-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-conversations-api-openapi.yml
- filename: agorapulse-drafts-api-openapi.yml
  format: yaml
  label: Agorapulse Drafts API
  slug: agorapulse-drafts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-drafts-api-openapi.yml
- filename: agorapulse-groups-api-openapi.yml
  format: yaml
  label: Agorapulse Groups API
  slug: agorapulse-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-groups-api-openapi.yml
- filename: agorapulse-health-api-openapi.yml
  format: yaml
  label: Agorapulse Health API
  slug: agorapulse-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-health-api-openapi.yml
- filename: agorapulse-items-api-openapi.yml
  format: yaml
  label: Agorapulse Items API
  slug: agorapulse-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-items-api-openapi.yml
- filename: agorapulse-media-api-openapi.yml
  format: yaml
  label: Agorapulse Media API
  slug: agorapulse-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-media-api-openapi.yml
- filename: agorapulse-organizations-api-openapi.yml
  format: yaml
  label: Agorapulse Organizations API
  slug: agorapulse-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-organizations-api-openapi.yml
- filename: agorapulse-pinterest-boards-api-openapi.yml
  format: yaml
  label: Agorapulse Pinterest boards API
  slug: agorapulse-pinterest-boards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-pinterest-boards-api-openapi.yml
- filename: agorapulse-profiles-api-openapi.yml
  format: yaml
  label: Agorapulse Profiles API
  slug: agorapulse-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-profiles-api-openapi.yml
- filename: agorapulse-replies-api-openapi.yml
  format: yaml
  label: Agorapulse Replies API
  slug: agorapulse-replies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-replies-api-openapi.yml
- filename: agorapulse-reports-api-openapi.yml
  format: yaml
  label: Agorapulse Reports API
  slug: agorapulse-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-reports-api-openapi.yml
- filename: agorapulse-workspaces-api-openapi.yml
  format: yaml
  label: Agorapulse Workspaces API
  slug: agorapulse-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/openapi/agorapulse-workspaces-api-openapi.yml
authorization_urls:
- https://api.identity.agorapulse.com/oauth/authorize
description: Agorapulse's REST API has no OAuth surface at all — it authenticates with a static per-user X-API-KEY and therefore has no scopes. The only OAuth surface is the remote MCP server, whose authorization-server metadata advertises exactly one scope.
docs: https://support.agorapulse.com/en/articles/12960496-model-context-protocool-mcp-integration-explained
flows:
- authorizationCode
kind: oauth-scopes
layout: scope
method: probed
name: Agorapulse Scopes
name_suffix: OAuth Scopes
note: ''
overview: 'Agorapulse publishes 1 OAuth 2.0 scope via the authorizationCode flow. Scopes are the fine-grained permissions an application requests at authorization time to act against the Agorapulse API on a user''s behalf.


  Tokens are issued from https://api.identity.agorapulse.com/oauth/token.


  This index is generated from the provider''s OpenAPI security definitions (and, where available, its documented scope reference) and refreshes on every APIs.io network build. Browse every provider''s scopes at [scopes.apis.io](https://apis.io/scopes/).'
provider_name: Agorapulse
provider_slug: agorapulse
schemes:
- flows:
  - authorizationUrl: https://api.identity.agorapulse.com/oauth/authorize
    code_challenge_methods:
    - S256
    flow: authorizationCode
    tokenUrl: https://api.identity.agorapulse.com/oauth/token
  issuer: https://api.identity.agorapulse.com
  name: MCP OAuth
  source: well-known/agorapulse-oauth-authorization-server.json
scope_count: 1
scope_names:
- read
scopes:
- description: The only scope advertised in scopes_supported. Agorapulse publishes no scope reference page, so there is no documented breakdown of what read covers; the REST API it fronts is itself described as read-only for reporting data.
  flows:
  - authorizationCode
  scope: read
slug: agorapulse-scopes
source_filename: agorapulse-scopes.yml
source_heading: OAuth Scopes
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://api.openmcp.agorapulse.com/.well-known/oauth-authorization-server\ndocs: https://support.agorapulse.com/en/articles/12960496-model-context-protocool-mcp-integration-explained\ndescription: >-\n  Agorapulse's REST API has no OAuth surface at all — it authenticates with a static per-user\n  X-API-KEY and therefore has no scopes. The only OAuth surface is the remote MCP server, whose\n  authorization-server metadata advertises exactly one scope.\napplies_to: https://api.openmcp.agorapulse.com/mcp\nschemes:\n- name: MCP OAuth\n  source: well-known/agorapulse-oauth-authorization-server.json\n  issuer: https://api.identity.agorapulse.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.identity.agorapulse.com/oauth/authorize\n    tokenUrl: https://api.identity.agorapulse.com/oauth/token\n    code_challenge_methods: [S256]\nscopes:\n- scope: read\n  description: >-\n    The only scope advertised in scopes_supported.\
  \ Agorapulse publishes no scope reference page, so\n    there is no documented breakdown of what read covers; the REST API it fronts is itself described\n    as read-only for reporting data.\n  flows: [authorizationCode]\n  sources: [well-known/agorapulse-oauth-authorization-server.json]\ngaps:\n- >-\n  No published scopes/permissions reference page was found on agorapulse.com or the help centre. The\n  single \"read\" scope is taken from the machine-readable metadata, not from documentation.\n- >-\n  scopes_supported on the protected-resource document (RFC 9728) is absent, so per-resource scope\n  requirements are not advertised.\nx-evidence:\n- {fetched: '2026-08-13', url: 'https://api.openmcp.agorapulse.com/.well-known/oauth-authorization-server', http_status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agorapulse/refs/heads/main/scopes/agorapulse-scopes.yml
summary_line: 1 scope · authorizationCode
tags:
- Social Media Management
- Social Media
- CRM
- Analytics
- Publishing
- Inbox Management
- Social Listening
token_urls:
- https://api.identity.agorapulse.com/oauth/token
---
